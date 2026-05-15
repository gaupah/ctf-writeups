![alt text](image.png)


![alt text](image-1.png)

when you click on the 'time' column header it will automatically arrange it chronologically

![alt text](image-2.png)

![alt text](image-3.png)

![alt text](image-4.png)

![alt text](image-5.png)

![alt text](image-6.png)

![alt text](image-7.png)

![alt text](image-8.png)

![alt text](image-9.png)

![alt text](image-10.png)

![alt text](image-11.png)

![alt text](image-12.png)

![alt text](image-13.png)

![alt text](image-14.png)

![alt text](image-15.png)

![alt text](image-16.png)

![alt text](image-17.png)

![alt text](image-18.png)

![alt text](image-19.png)

![alt text](image-20.png)

![alt text](image-21.png)

![alt text](image-22.png)

![alt text](image-23.png)

![alt text](image-24.png)

you can use this command too:
![alt text](image-25.png)

then convert hex to base64 strings and then decode it 

you can run this tshark command to get the o/p directly:


tshark -r myNetworkTraffic.pcap -T fields -e frame.time_epoch -e tcp.payload 2>/dev/null \
  | sort -k1 -n \
  | awk '{print $2}' \
  | while read hex; do
      python3 -c "import base64; b64=bytes.fromhex('$hex').decode(); print(base64.b64decode(b64).decode('latin-1'))" 2>/dev/null
    done


![alt text](image-26.png)

### Flag: 
```
picoCTF{1t_w4snt_th4t_34sy_tbh_4r_f318db22}
```