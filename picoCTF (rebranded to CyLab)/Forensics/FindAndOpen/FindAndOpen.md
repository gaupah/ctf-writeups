![alt text](image.png)

![alt text](image-1.png)

![alt text](image-3.png)

![alt text](image-4.png)

filtering out the ethernet packets:
![alt text](image-2.png)

![alt text](image-5.png)

from packet 49 to 57, on protocol the following message has been transmitted:

![alt text](image-6.png)

```
PBwaWUvQ1RGesabababkjaASKBKSBACVVAVSDDSSSSDSKJBJS
```

![alt text](image-7.png)

from packet 58 to 65, on protocol 46, the following message was transmitted:
![alt text](image-8.png)

```
PBwaWUvQ1RGe1 Maybe try checking the other file
```



### re-approached the challenge:

![alt text](image-9.png)

![alt text](image-10.png)

this packet is the only with a different protocol, so let's analyze it:
the highlighted text:
```
VGhpcyBpcyB0aGUgc2VjcmV0OiBwaWNvQ1RGe1IzNERJTkdfTE9LZF8=
```

decoding the message gives us:
![alt text](image-11.png)

```
This is the secret: picoCTF{R34DING_LOKd_
```

in one of the packets, it hinted the flag has been split, so let's assume the other part of this flag is somewhere in the zip file.


![alt text](image-12.png)
so the secret pass to unlock this zip file was `picoCTF{R34DING_LOKd_`

![alt text](image-13.png)

Flag:
```
picoCTF{R34DING_LOKd_fil56_succ3ss_0f2afb1a}
```

ezzzz

