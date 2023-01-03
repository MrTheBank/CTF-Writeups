# SECUREiNFO (Mini Challenge) - Network
> Analyze this network traffic and find which port is opened.  
>  
We will use Wireshark to analyze this network traffic.   
![image](https://user-images.githubusercontent.com/16158569/210325101-d58969e1-984a-4160-ade4-3b1d5e8fcdd0.png)   
This required basic network knowledge so what we need to know are   
Closed port - Respond with RST,ACK flags.   
Opened port - Respond with SYN,ACK flags.   
<br />
Now we will filter Wireshake to show only packet that contain SYN,ACK flags.   
Using this filter   
`tcp.flags.syn==1 and tcp.flags.ack==1`   
![image](https://user-images.githubusercontent.com/16158569/210326648-ff9b934e-d16a-40e1-9cbc-5a9cd283323e.png)   
Done. We found opened port packet.   
192.168.56.103:37656
