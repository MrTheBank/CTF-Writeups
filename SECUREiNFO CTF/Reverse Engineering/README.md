# SECUREiNFO (Mini Challenge) - Reverse Engineering
Let execute this binary file.   
![image](https://user-images.githubusercontent.com/16158569/210327821-8331a6f7-4283-4943-8a5f-0815f81971d5.png)   
It seem like we can't do anything here. Can't even send kill signal to process.   
Let reverse this binary file by using Ghidra but first we need to know binary type.   
![image](https://user-images.githubusercontent.com/16158569/210328630-d588577b-3b4d-471c-a995-711c73aeb1b7.png)   
ELF 64-bit LSB   
Now set version to decompile this binary.   
![image](https://user-images.githubusercontent.com/16158569/210328792-308a86f4-17a0-41e8-9ea0-082bf2bc19ca.png)   
Search each function and find function that might related to flag answer.   
![image](https://user-images.githubusercontent.com/16158569/210342008-91e0afb3-1bde-4b65-a9e5-1f446143d8ce.png)   
Look like it's hexadecimal, let convert it into character using Python.   
![image](https://user-images.githubusercontent.com/16158569/210343394-99716a92-81c5-45ef-9366-a1bfba940697.png)
We got flag!   
`flag{gReaT!!!_Is1THard?}`
