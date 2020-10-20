### ** CHALLENGE PROMPT ** :

What is the name of the executable in the malicious url?

Again , we are given a .pcap file to analyse that had loads of packets. Here's some of them to get an idea :

![general](https://user-images.githubusercontent.com/73142671/96652004-b295e480-133e-11eb-975d-f0d02123e463.png)

In this scenario , we specifically filter for the **http** protocol , since it's unencrypted by design.
Thus, we get the following :

![http](https://user-images.githubusercontent.com/73142671/96652116-f12b9f00-133e-11eb-8750-9acd358cf8aa.png)

Flag is : flag{solut.exe}
