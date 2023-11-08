# Keygenme-py


I started off by having a quick glance at the code.
Then looked into it in detail. 
The first few lines made it clear what the format of the flag would be.
<img width="586" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/37fa2b11-ce18-4c27-9653-443c3eceebcc">

I would have to get the dynamic1_trial part to get the flag.

Then there was this menu with 4 options. After studying the code for the 4 different options I concluded that the license part is where I would have to look.
Only this piece of code was using the key.

In the program the user is supposed to enter a key to login. The program then checks the inputted key. To get the key, I would have to see what the code is comparing the inputted key to.
First there was a check for the length and then for the static part. i already had both of these.

<img width="377" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/f53d31bc-82ed-458a-bf5a-72438223f6f5">

The part of interest was the dynamic part. And it had a lot of things I hadn't seen before.

<img width="362" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/aa858e86-f5dd-4a2d-8a66-06254ebdb38a">

First of all I looked up hashlib and sha256.
Hashing is the process of transforming a key into another vakue using a particular function.
The hashlib library of python offers different functions for hashing. The one used here was sha256.

I also looked up hashdigest and learned that it is used to convert hash values into a hexadecimal string. The code here is basically taking particular values from this string. 
And the username is the string being hashed. 
Now I would have to get these values.

<img width="590" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/8576aa4a-3a9e-47da-8255-c17b686ebca7">
I tried to do this. 
But got an error that strings must be encoded before hashing.
When I looked up the error on google, I found I could do the hashing if the string was bytes object. This was already done in the code. I just didn't realise that b meant converting it into bytes.

<img width="501" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/e729554a-77ec-4b9e-9dd8-c15fb531579b">

So I printed all the values of the indexes of the string that the code was comparing the entered key with. 
This would complete the missing part of the key.

picoCTF{1n_7h3_|<3y_of_f911a486}

Got the flag!



