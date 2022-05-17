## Lab Report 3  
**#1: Streamlining ssh Configuration ->**  
After opening the .ssh folder from the File Explorer into VScode, I wrote the following code:  
![Lab Report #3 CSE 15L Streamlining ssh Configuration Code](https://user-images.githubusercontent.com/103283657/167768078-92c2fc98-89bb-44f5-8004-bc53e9936b56.png)     
  
Which resulted in the following output:  
![Lab Report #3 CSE 15L Streamlining ssh Configuration Terminal Output](https://user-images.githubusercontent.com/103283657/167768379-2d6e13b6-e3e7-44bc-a200-df7427ed7a69.png)  
  
Now we can work with our easier login information to work in the server!:  
![ieng6 SCP File Lab Report #3 CSE 15L](https://user-images.githubusercontent.com/103283657/168864502-4f1ed4f8-55b9-4a49-84d4-7a7e5fee641e.png)  
  
  
**#2: Setting up Github Access from ieng6**  
I stored the public ssh key in github, which looks like this:  
![Public Key ieng6 CSE 15L Lab Report #3 Screenshot](https://user-images.githubusercontent.com/103283657/168690065-598ad911-34e1-496a-9e6c-6a52ea75ac17.png)  
  
This is what my private key looks like:  
![Private Key CSE 15L](https://user-images.githubusercontent.com/103283657/168888015-c424603d-301e-4f43-9015-571b7d678c82.png)  
  
I can also run git commands in the remote server, as seen here:  
![Git Commands in ieng6 CSE 15L Lab Report #3](https://user-images.githubusercontent.com/103283657/168866111-c76d0f74-eb12-4aa6-beaf-262c32999aab.png)  
  
[Changes made towards Github may be seen here](https://github.com/Santiago-Duque/skilldemo/commit/99c9625522335429a05236c284bf0664caa4ed46)

  
**#3: Copy Whole Directory With scp -r**  
I copied my whole markdown-parser directory into my ieng6 account as seen here:  
![Copy Whole Directory Lab Report #3 CSE 15L](https://user-images.githubusercontent.com/103283657/168692016-0935a5ac-2e0e-4c28-9dc6-4a8cbbad508a.png)  
  
You can see that the directory appears in the ieng6 account:  
![Logging Into ieng6, Running Commands CSE 15L Lab Report #3](https://user-images.githubusercontent.com/103283657/168693487-7b23f0e3-094d-4975-a576-8816afe15763.png)  
  
This is what happens when I combine everything to copy the whole directory!:  
![Scp CSE 15L Lab Report #3](https://user-images.githubusercontent.com/103283657/168694693-ea893c35-5141-4195-b4dd-3a1f3ea75116.png)  

