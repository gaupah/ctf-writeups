![alt text](image.png)


![alt text](image-1.png)

![alt text](image-2.png)

the SSID is `Gone_Surfing`
the BSSID is `00:5f:67:4f:6a:1a`

using the command:
```
aircrack-ng -w /usr/share/dict/rockyou.txt -b 00:5f:67:4f:6a:1a wpa-ing_out.pcap
```
![alt text](image-3.png)

we found the key as:
```
mickeymouse
```

Flag:
```
picoCTF{mickeymouse}
```