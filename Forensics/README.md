# Digital Forensics 
## G&P List 
Just Open the File and Capture the flag . Submission in MD5

* First thing thought of ofc is to use the command exiftool to see more info about the file. 

![Image](./assets/Capture1.JPG)

We can see clearly that the file type is Zip. Let's unzip it. 

![Image](./assets/Capture2.JPG)

The flag is in Flag.txt 


## Hidden Message 
A cyber Criminal is hiding information in the below file . capture the flag ? submit Flag in MD5 Format

* Just use exiftool command and instantly get the flag 

![Image](./assets/Capture3.JPG)


## Cypher Anxiety 
An image was leaked from a babies store. the manager is so annoyed because he needs to identify the image to fire charges against the responsible employee. the key is the md5 of the image

* Download and unzip the file, we get a pcap file which is used to capture network traffic. 
* Then, we open it using wireshark. 
* If we navigate a little through the packets we'll find this : 

![Image](./assets/Capture4.JPG)

* So, let's see what strings will tell us : 

![Image](./assets/Capture5.JPG)

As the message says, we should filter with port number 7070 and use cryptcat to decrypt the data sent. 

![Image](./assets/Capture6.JPG)

Then follow tcp stream and save it as raw. 

![Image](./assets/Capture7.JPG)









