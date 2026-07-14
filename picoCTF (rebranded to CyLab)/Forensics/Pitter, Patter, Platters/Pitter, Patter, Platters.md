![alt text](image.png)

![alt text](image-1.png)

![alt text](image-2.png)

![alt text](image-3.png)

![alt text](image-4.png)

![alt text](image-5.png)

if you read it in reverse, you can get the flag:

![alt text](image-6.png)

using the command:
```
blkcat suspicious.dd.sda1 2049 | xxd -p | tr -d '\n' | xxd -r -p | rev
```

Flag:
```
picoCTF{b3_5t111_mL|_<3_f2136893}
```


