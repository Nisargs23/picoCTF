# SafeOpener
This challenge was pretty easy. We are given a program file which basically gives us 3 attempts to enter the correct password.

<img width="487" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/c61acafc-eb05-43f1-8c26-8ee13f55156d">


From the program it is evident that the entered password is first encoded and then compared with a particular string.
The encoding is also made pretty clear. It is base64.

<img width="266" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/31e6c87c-bf87-4381-9638-9df7ad2034c0">

Once I entered the string being compare into a base64 decoder, I got the flag.

Fairly straightforward this one.
picoCTF{pl3as3_l3t_m3_1nt0_th3_saf3}
