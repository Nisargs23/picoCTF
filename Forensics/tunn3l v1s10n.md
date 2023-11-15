#tunn3l v1s10n

In this channel, there was a file of unkonwn type. First thing I tried to do was to try and find out what kind of file it was.

<img width="475" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/a5aa5ca8-3122-478b-adcb-1dcfea06b6bf">

That didn't help. And trying to see the contents gave a whole lot of gibberish.

So I searched how to find out the file type and people were putting the file into a hex editor to find out the type of file.

I did the same and from what I learned, the first 2 letters being BM indicates that it is a bitmap file.

<img width="546" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/30a95fa4-b4cc-4da8-9663-1b986b360825">

Bitmap files are used to store images and they have a .bmp extension.

I downloaded a hex editor for this and saved it as a bitmap file. It didn't open, so there was something wrong with the file.

As per a few websites and videos, the header had incorrect values and would have to be changed to get an image.

So I changed the faulty looking values. Which I honestly could not tell myself. I had to get help.

![image](https://github.com/Nisargs23/picoCTF/assets/148000598/f32e4ee2-e320-4b5c-9d42-c69d13bd690a)

and it gave this which was not the answer.

The image is incomplete, there should be more to it. According to a video I watched, the height and width could be changed in the hex editor.
The format in which the data is stored is called little endian and is a format for hex numbers.

Now I messed around with the hex values a lot

And more often than not ended up with images like this

![image](https://github.com/Nisargs23/picoCTF/assets/148000598/73958d30-4d6c-4b58-a3ba-6fc3004a2f51)

Then finally I found out which value was working properly

![image](https://github.com/Nisargs23/picoCTF/assets/148000598/bcd4d772-8c93-416c-87bf-9dd69227b2fe)

![image](https://github.com/Nisargs23/picoCTF/assets/148000598/78371ac3-9597-4674-9a79-f475c5f23d79)

picoCTF{qu1t3_a_v13w_2020}
