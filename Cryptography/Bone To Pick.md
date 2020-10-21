### **CHALLENGE PROMPT** :

We intercepted network traffic between two suspected DEADFACE actors. The problem is,we have no idea what we're looking at. 
We think it might have critical information. See if you can find the critical information from the link below and submit the flag.

We are given a link to a pastebin which contains a single line of a really long string : 

![Screenshot_2020-10-21 _9j_4AAQSkZJRgABAQEAeAB4AAD_4QAiRXhpZgAATU0AKgAAAAgAAQESAAMAAAABAAEAAAAAAAD_2wBD - Pastebin com](https://user-images.githubusercontent.com/73142671/96654484-15d64580-1344-11eb-9c1d-668ffcb712ff.png)

The string goes on for quite a while .
Looking around we find that the given string is an image encoded in base64.

Repairing the malformed base64 string and converting it to an image with online tools , we get this :

![flaga](https://user-images.githubusercontent.com/73142671/96654849-deb46400-1344-11eb-9e9a-9eec3027912c.jpg)

Thus , the flag is : flag{angrybones}
