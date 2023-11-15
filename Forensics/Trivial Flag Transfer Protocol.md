# Trivial flag transfer protocol

tftp stands for trivial file transfer protocol which basically allows exchange of files between machines.

The file in this challenge was a pcapng file. This kind of file stores data about a network. This data is used to analyse the network characteristics. I learned all this only beacuase of the challenge.
To open this file, I installed wireshark, as few of the references I read had wireshark in them.

There were tftp and arp I followed instructions to export the tftp files.

After being exported, there were a few files, Three images and a few text files.

<img width="508" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/b2e8847c-cf79-4a02-8fed-a9cc0165b500">

The first one I opened was obviously instructions. It was encrypted so I tried a few ciphers like caesar. It was a rot13 cipher.

This was what it said TFTPDOESNTENCRYPTOURTRAFFICSOWEMUSTDISGUISEOURFLAGTRANSFER.FIGUREOUTAWAYTOHIDETHEFLAGANDIWILLCHECKBACKFORTHEPLAN

TFTP DOESNT ENCRYPT OUR TRAFFIC SO WE MUST DISGUISE OUR FLAGT RANSFER. FIGURE OUT A WAY TO HIDE THE FLAG AND I WILL CHECK BACK FOR THE PLAN

That points to the plan file
The plan file was also encrypted in rot13

It said IUSEDTHEPROGRAMANDHIDITWITH-DUEDILIGENCE.CHECKOUTTHEPHOTOS

Now naturally I would have to check out the program. I tried installed the program, and had to look up the commands to do so.

<img width="608" alt="image" src="https://github.com/Nisargs23/picoCTF/assets/148000598/4f9bea95-4e59-4042-bdfc-b1d6694234e7">

I wasn't able to install at first, but then I didn't have to.I came across what was being installed :steghide.

I looked it up. Steghide is basically a program that enables a user to hide data in images.
Which makes sense for our problem. I would have to run the Images through steghide.

Now I tried to install steghide but there was some error, and it was taking a really long time. I just used an online decoder.

The first two images didn't have any flags. The third image gave the flag

picoCTF{h1dd3n_1n_pLa1n_51GHT_18375919}
