# gdb baby step 1

Well for this challenge first I had to lok up what gdb is.
It stands for GNU debugger.
From what I understand it basically lets us see what goes on in the program in a more detailed way.
First to use gdb, had to learn how to access files on my computer using wsl.
And then of course install gdu.

<img width="516" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/8141cc0f-d140-412c-851f-378cbd5d4f0c">

I messed around in gdb just exploring it.

<img width="608" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/ae8ec13c-f92d-446e-a2a8-727789573d02">

Now the question said that the register was at the end of the main function. A google search was sufficient to know that info functions would list all the functions.

The questions then said to disassemble the file. Turns outh the command to disassemble the file is disassemble. 

<img width="475" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/a4c0d9ff-3715-46f6-94fc-ae4462051253">

<img width="411" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/0ae57a94-19b3-41e1-9568-684374781c9f">

coverting the hexadecimal to decimal gave the flag.
picoCTF{549698}
