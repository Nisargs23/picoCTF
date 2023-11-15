# miniRSA

There was a plain text file in this challenge.

<img width="709" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/44d9898a-26c1-4d95-9433-3de711d44001">

I looked up what rsa was. 

It is basically an encryption algorithm. It works by picking large numbers and calculating the cipher.

The formula is basically c=m^e % n
where c is the cipher and m is the data to be encrypted.

In the challenge, we are given the value of e, c and n, and the value of e is small i.e. 3

Upon computing the cube root of c, we get a value. I couldn't find any cube root finders for such large numbers online, so I used a program to find cube root.

This value when converterd to hex and subsequently to ascii, gives the flag


picoCTF{n33d_a_lArg3r_e_d0cd6eae}
