![alt text](image.png)

![alt text](image-1.png)

![alt text](image-2.png)

![alt text](image-3.png)

![alt text](image-4.png)

![alt text](image-5.png)

The .ash_history shows exactly how the flag was encrypted:
```
openssl aes256 -salt -in flag.txt -out flag.txt.enc -k unbreakablepassword1234567
```

![alt text](image-6.png)

![alt text](image-7.png)

Flag:
```
picoCTF{h4un71ng_p457_0a710765}
```