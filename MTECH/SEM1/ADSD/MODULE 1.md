- [ ] PROCESSOR ARITHMETIC
	
- [x] Two’s Complement Number System – Arithmetic Operations
	if negative convert to binary and add 1
	if positive use as is

	consider a - b as a +(-b)
	and if result MSB = 1 
	do complement again to find decimal part and use as -ve
	Range of two's complement is from -2^(n-1)  to 2^(n-1) -1
- [ ] Floating Point Number system – IEEE 754 format & POSIT,  
	
- [ ] Basic binary codes.
	- [ ] BCD
	    - [x] BCD Addition and correction
	    - [x] BCD encoding and decoding
	    - [ ] BCD Limitations
	    - [ ] BCD advantages
	- [ ] XS-3
		- [ ] Addition
		      convert to XS-3 equivalent
		      add each nibble independently 
		      if a nibble generates a carry add 0011(3) to it
		      if the nibble doesn't generate a carry subtract 0011(3) from it
	 **non weighted**
	  adds 0011 to BCD code to generate the corresponding XS-3
	  **SELF complementing as well as SEQUENTIAL**
	  if the 9's complement of a number is the bit inverted form for that number then it is a self complementing code 
	  if current code + 1(binary) = next code then it is a sequential code
	- [ ] GRAY
	      unit distance each element is one bit change away from the previous/next bit
	     **i.e Two consecutive bits differ by only one bit ** 
	      reduces error probability when compared to multiple bit changes per 
		      example is a mechanical shaft encoder(position sensor)
		 Xor gate is used to generate the Gray code from Binary|
		 **REFLECTIVE - first half is mirror image of the second half Excluding MSB
		 Binary to Gray
		 G3 = B3
		 G2 = B3 XOR B2
		 G1 = B2 XOR B1
		 G0 = B1 XOR B0
		 
		 GRAY TO BINARY
		 B3 = G3
		 B2 = G2 XOR B3
		 B1 = G1 XOR B2
		 B0 = G0 XOR B1
	- [ ] HAMMING Code
	      2^k >= m+k+1
	      m - number of data bits
	      k - number of parity bits
	      1 state for no error
      
	