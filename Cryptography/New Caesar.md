# New Caesar

In this challenge we were given a python file which had a code for encrypting a string.

On going through the code, we can see two main processes occurring, one is the shift and the other is the b16_encode function.

<img width="358" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/bd607f38-1310-499d-811a-165caf9beb3d">

Now the b16_encode is basically taking the flag and converting it into binary. It then splits the binary into 2 parts and hence 2 numbers. The entered flag is then coded as the 2 letters that would be obtained from the numbers.

These numbers are positions in the string alphabet which is basically the first 16 alphabets.

Now the key lies between these 16 alphabets and we can check each letter to get the flag.

I had to write a code to decode the b16_encode function. It took a little help to do so.

<img width="592" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/e4c149ae-c8f1-4e3b-ad27-8e7eea9c4235">

<img width="485" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/ab8fb7e1-7b80-464e-8169-5d9c826d8ed7">

picoCTF{et_tu?_1ac5f3d7920a85610afeb2572831daa8}
