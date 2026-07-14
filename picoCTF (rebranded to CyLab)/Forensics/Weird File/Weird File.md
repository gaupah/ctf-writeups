![alt text](image.png)

yt video:
https://www.youtube.com/watch?v=Y7IJjnLGqTQ

<--! talk bout .docm, word 2007 macros>

i am on arch, so I'll be using libre office to work on this document 

![alt text](image-1.png)

this is what I see, when I open the document in libreoffice

![alt text](image-2.png)


will try to edit macros:
go to tools > Macros > Edit Macros
![alt text](image-3.png)

in the highlighted section you can see that, they must've mistyped `\` before `"` and hence the macro didn't work, this macro is basically a python scripts... which can later be decoded to find the flag

![alt text](image-4.png)

Flag:
```
picoCTF{m4cr0s_r_d4ng3r0us}
```

