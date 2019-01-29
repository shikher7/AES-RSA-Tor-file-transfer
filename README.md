# aes-rsa-tor-file-transfer
As technology advances there is an increase in the amount of data being transferred over the network. One of the principle challenge that is faced is security. Security is achieved by encryption; In this project, a AES symmetric block cipher is initially used to encrypt the file, the key obtained from the AES encryption is encrypted again using bit RSA algorithm. Similarly, the decryption is done using RSA algorithm to obtain the key which is used to decrypt the message using AES algorithm. AES is a symmetric algorithm that uses only a private key and RSA is an asymmetric encryption system that works with two different keys: A public and a private key. Both work complementary to each other, which means, when a message is encrypted with one of them can only be decrypted by its counterpart. This combination of algorithms provides better security and efficiency. The file served on a Tor server from which anyone can download by accessing the onion link but only person with private key will be able to decrypt the file. 

IMPLEMENTATION 

We have used these two techniques in this file sharing project and also used tor services for securely sharing files.

Step 1: Browse the file to be encrypted. 

Step 2: Now will apply AES encryption on browsed file using randomly generated key. 

Step 3: From AES encryption will have key and encrypted file. 

Step 4: Key generated from AES will be encrypted using RSA and it will use public key of receiver to encrypt given data (key from AES). 

Step 5: Now we have encrypted data and encrypted key. 

Step 6: Now tor URL can be generated which can be used for file (encrypted file) sharing on any system having tor environment. 

Step 7: To decrypt the file, receiver will use its private key which only he have, receiver can use onion link on tor browser and can download encrypted file. Now he can decrypt the file using its private key.

Step 8: Receiver have decrypted file without any security breach, while sharing the file between sender and receiver. 
