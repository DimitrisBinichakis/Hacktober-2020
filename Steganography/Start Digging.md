### **CHALLENGE PROMPT** :

There's a secret buried here, but we need help finding it. Supposedly, there's a flag hidden deep
within this image. But how far down do we need to dig?

![steg06](https://user-images.githubusercontent.com/73142671/96652950-ac086c80-1340-11eb-934c-920e12b36ca5.jpg)

Running 

  > binwalk image.jpg
  
 We get this : 
 
 ![binwalksteg06](https://user-images.githubusercontent.com/73142671/96653028-d78b5700-1340-11eb-90ad-d2aeaafcec3b.png)

We can see something is hidden inside the original image , lets run foremost to extract it .

  >foremost image.jpg
  
Creates a new output directory . Inside there we find two things : 00000000.jpg  00000230.jpg

00000 is the original photo 0000230 is this new photo. Let's run EOG to view 00000230.jpg

![0230EOG](https://user-images.githubusercontent.com/73142671/96653160-1faa7980-1341-11eb-8f53-182c04d03b13.png)

'binwalk' allows extracting the embedded data/files etc. when provided '-e' attribute/flag but that won't work in this scenario.
We will have to use '--dd' flag/attribute to get the image.

  > binwalk --dd '.*' 00000230.jpeg

![binwalk--dd](https://user-images.githubusercontent.com/73142671/96653456-d0187d80-1341-11eb-9423-69ac961bf091.png)

We get a new file , "_00000230.jpg.extracted" created from binwalk .
Inside that directory , we get 4 new images :

  0  B8  C  C4

Viewing B8 with EOG reveals the flag :  

![flag](https://user-images.githubusercontent.com/73142671/96653403-ac553780-1341-11eb-9f5c-a0121cce67b5.png)
