# SECUREiNFO (Mini Challenge) - Digital Forensic
We have 2 files, TheMatrix.png and intel.txt that have following content   
```
1. Zip password is the Plus Code of CYNIUS Cybertech and Consulting Co., Ltd.
2. SHA512 Hash the dog and you get the flag.
```   
Well we might use later   
Let open this png file   
![image](https://user-images.githubusercontent.com/16158569/210321530-16e1bcca-2f9e-4025-bf38-99b20411f25b.png)   
It seem like we can't open this file, let check the file format first if it's really image file.   
![image](https://user-images.githubusercontent.com/16158569/210321677-d2b540a1-514b-4839-8e0e-4e7bb0f2a970.png)   
Ah! Gzip file, let extract gzip file with `tar xvf TheMatrix.png` command.   
![image](https://user-images.githubusercontent.com/16158569/210321998-f1968855-ec54-4fe1-9651-ce8364df7e6b.png)   
Now we got layer1.psd file but I don't think it's real psd file, let check file format again.
![image](https://user-images.githubusercontent.com/16158569/210322148-d1f6cf00-b9c7-46b6-9b0a-a10df55162dc.png)   
Zip file, let extract zip file with `unzip layer1.psd`   
![image](https://user-images.githubusercontent.com/16158569/210322360-09a5bd28-2258-4799-8537-41662cab212e.png)   
But this file seem like it's locked so what is the password?   
Remember intel.txt file that give us a hint?   
```
1. Zip password is the Plus Code of CYNIUS Cybertech and Consulting Co., Ltd.
```   
What is Plus Code? Let google it.   
![image](https://user-images.githubusercontent.com/16158569/210322597-9dd8ebdc-bdee-43dc-b17d-c1ad93135850.png)   
Now we will need to find plus code of CYNIUS Cybertech and Consulting Co., Ltd. by using Google Map.   
![image](https://user-images.githubusercontent.com/16158569/210322788-19eff80b-0ccb-44f7-9cf5-db577fce5e69.png)   
Now we got plus code, let try it to unlock zip file.   
![image](https://user-images.githubusercontent.com/16158569/210323065-349b9129-d011-4ae9-8099-185d23736cf3.png)   
The password worked! And now we have doggogo.jpg file.   
Next step we will have to hash this image file by using `sha512sum doggogo.jpg`   
![image](https://user-images.githubusercontent.com/16158569/210323742-d5f7a80a-49ee-4b4f-9d05-38c01d446b75.png)   
Finally, We got the flag.
`5bd4a140554b98867659c5f945875f7cb639b53f165ee8da468d3a2d9eb3f43ab7298eb631ce6dbe48b7932768b70f71c232809e122f6cfb2dba1e460457296d`
