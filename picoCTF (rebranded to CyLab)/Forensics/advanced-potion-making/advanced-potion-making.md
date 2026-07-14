### this challenge was a pain, so it will take some time to write a detailed writeup

![alt text](image-1.png)

![alt text](image.png)

![alt text](image-2.png)

the file signature looks similar, but looks like it's slightly corrupted

we'll have to replace these bytes (highlighted ones) with the correct ones:

![alt text](image-3.png)

the correct file signature for PNG is:
```
89 50 4E 47 0D 0A 1A 0A
```

so the changed bits look like:
![alt text](image-4.png)

export the file:
![alt text](image-5.png)


hmm...it still didn't save as a PNG file, so there must be some kinda corrupted data still reamining to be fixed

okay, nvm I checked in my file explorer
![alt text](image-6.png)

uhhhh, still won't open...
![alt text](image-7.png)

so it seems I need to check and fix the bytes for IHDR:

![alt text](image-8.png)

![alt text](image-9.png)

![alt text](image-10.png)
finally T_T

okay but it still says, there is an error

uhh I am just gonna start all over:

![alt text](image-12.png)

so the completely changed header is (16 bytes):
```
89 50 4E 47 0D 0A 1A 0A 00 00 00 0D 49 48 44 52
```

![alt text](image-13.png)

![alt text](image-14.png)

opening the file gives us this, hmm...

![alt text](image-15.png)

if you look carefully, you can see some light text, let's use some filters:

![alt text](image-16.png)

Flag:
```
picoCTF{w1z4rdry}
```