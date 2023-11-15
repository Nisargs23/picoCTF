# MacroHard WeakEdge

This challenge had a .pptm file.
I opened it in powerpoint, but there was only a single slide with content. The rest of the files were empty. 

<img width="908" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/ec0a1a1a-2eb6-400d-9bcb-688a688d5061">


As it was a .pptm file it had macros. Now I didn't know this earlier, but many MS Office documents are a collection of files and folders that can actually be extracted. The command to do yhis was unzip.

<img width="647" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/ba9acf75-1809-4208-a0c6-08d164c04383">

Now there were quite a few files in this extracted bunch of files.

<img width="948" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/59752131-a027-483f-9898-c93d6b377922">

I opened a few files. Most of the contents of these files were of no use.Then I saw the last one. It had hidden in the name.
So that would probably be the one.

It had a string which was encrypted

<img width="950" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/336a784d-3697-4c87-8f3d-2b495f65eb98">

It took me quite a while to figure out what the encryption was. It was in base64. Upon conversion, I got the flag.

picoCTF{D1d_u_kn0w_ppts_r_z1p5}
