### **CHALLENGE PROMPT** :

What MYDDNS domain is used for the post-infection traffic in RATPack.pcap?

The .pcap file to analyse is the same as for the first challenge.

In order to solve this one , we filter for **DNS** in wireshark.Thus, we get this : 


![2020-10-17_18-43](https://user-images.githubusercontent.com/73142671/96652321-57b0bd00-133f-11eb-8b5a-7972ea8ebbef.png)

From the packets above , we conclude that the flag is : flag{solution.myddns.me}
