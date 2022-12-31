# Digital Forensic 06
Import windows XP.ova into VMWare or VirtualBox.   
![image](https://user-images.githubusercontent.com/16158569/193491285-79f72f72-3859-4ef7-99d0-a37d48254bf2.png)  
You will found that there are 2 user accounts that locked.   
Download [HirenBoot](https://www.hirensbootcd.org/download/) and boot into VM to change password using NT Password Edit tool.   
![image](https://user-images.githubusercontent.com/16158569/193491752-b1a29580-0a40-4891-8275-09b0de26b8dd.png)  
After we changed the password, login into winxp with new password.     
Then use keyword to find the secret files in recursive.   
![image](https://user-images.githubusercontent.com/16158569/193492073-9b0d463b-3fb4-47c6-96b6-9a4f512c9aaa.png)  
![image](https://user-images.githubusercontent.com/16158569/193492136-0ba48653-18aa-4f64-b359-be7582c5c469.png)
hackernote?! Must be secret we are looking for.   
![image](https://user-images.githubusercontent.com/16158569/193492180-796eafb2-f2a6-4df6-b871-15e13a717ec1.png)  
Yes we got the flag!   
`tctt2022{Expl0it_windows/smb/ms08_067_netapi}`   
