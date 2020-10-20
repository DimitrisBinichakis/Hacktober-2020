### **CHALENGE PROMPT**:

The malware uses four different ip addresses and ports for communication, what IP uses the same port as https?

We were instructed to use the same .pcap file as Ecorps child 1.

With that in mind , knowing that **https default port is 443** , using wireshark and going to
endpoints -> tcp we get this.

![2020-10-17_18-48](https://user-images.githubusercontent.com/73142671/96651748-208ddc00-133e-11eb-8a14-2a32e9516971.png)

Since we know that the port we are looking for is 443, that narrows down our options by a lot . 

Through manual iteration , we get the flag 

flag{213.136.94.177}
