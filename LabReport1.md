# ieng6 Tutorial for Incoming CSE 15L Students  
Welcome to the `CSE 15L` course! Here is how to log into the CSE 15L account on ieng6:  
1. **Install the code editor** [`VScode`](https://code.visualstudio.com/). This is what you should see after installing: 
![Installing VScode CSE15L](https://user-images.githubusercontent.com/103283657/163917919-690dc8c7-2756-4704-bf8c-4fe389b6ff73.png)  
  
Description: VScode is an offline editor that is essential in providing quick updates made to your code. After I installed the code editor, 
I went to the top-right corner and selected: File > New File. This action creates a file for you to write your code in.  
  
2. **Connect Remotely** by writing your account details in the terminal. Assuming it is your first time connecting to the server:  
type: **ssh cs15lsp22zz@ieng6.ucsd.edu**. Make sure to replace the `zz` with the actual letters of your account. A question regarding a  
fingerprint may pop up, so click `yes`. After this, you will be prompted to enter your password. **NOTE**: you will not be able to see  
your password when you enter it, as the password is encrypted for security. If you followed the steps correctly, this is what you should see: ![Connecting Remotely CSE 15L](https://user-images.githubusercontent.com/103283657/163917317-7e03259b-a892-437c-bd51-011b2807ab07.png)  
  
Description: Connecting to the server will allow you to run commands to play with the files within the server, as seen in further steps.  
  
  
3. **Run some commands!**: There are various commands that you can run in the terminal to see information about your files, such as:  
-cd ~  
-cd  
-ls -lat  
-ls -a  
I tried the command ls -lat, and look what popped up!  
![Running Some Commands CSE 15L](https://user-images.githubusercontent.com/103283657/163918189-311c28fa-acca-4cce-bd1e-33e280cc34f4.png)  
Description: There are various commands you can use, and each command brings up different information. For example, a lot of information popped
up when I ran the ls -lat command!  
  
4. **Move some files with scp!**: The `scp` command copies files from your computer (**the client**) to a remote computer  
(**not logged into the ieng6 server**)  Let's make a sample file to move! Make a file in VScode with the following contents:  
class WhereAmI {  
  public static void main(String[] args) {  
    System.out.println(System.getProperty("os.name"));   
    System.out.println(System.getProperty("user.name"));  
    System.out.println(System.getProperty("user.home"));  
    System.out.println(System.getProperty("user.dir"));  
  }  
}  
Run this code in the terminal by typing: `javac WhereAmI.java` |after clicking enter type: `java WhereAmI`  
Next Step: type: `scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/`  
log in with **ssh cs15lsp22zz@ieng6.ucsd.edu** again, and then type `ls`. This is what you should see: ![Moving Files With SCP CSE 15L](https://user-images.githubusercontent.com/103283657/163918613-695c517a-715e-4775-98a8-a2a426c5d19d.png)  
Description: I created a file to transfer from my computer to a remote server using scp. It was a similar process as the beginning steps, as I had to log in to the ssh account again!  
  
5. **Setting an SSH Key**: This is what you should see: ![Setting Up SSH Key CSE 15L](https://user-images.githubusercontent.com/103283657/163918880-f8d53b0a-ccf3-44b3-b2d0-8416cd960566.png)  
Description: the ssh-keygen command creates a public key and private key; saving the hassle of needing to keep logging in to the ssh account within the terminal! In the terminal, type: `ssh-keygen OR ssh-keygen -t ed25519`. You will see it says: Enter file in which to save the key (/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa. Replace <user-name> with the username on your computer, and click enter twice for the two prompts that pop up after such action.  
  
6. **Optimize Remote Running**: Here's an example of optimization: ![Optimize Remote Running CSE 15L](https://user-images.githubusercontent.com/103283657/163918946-761a77b5-3489-42de-ba7c-af8d2b89edf9.png)  
Found ways to run commands in the terminal more efficiently! Saves time and the number of writing needed for a command to run!  
  
