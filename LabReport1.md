# ieng6 Tutorial for Incoming CSE 15L Students  
Welcome to the `CSE 15L` course! Here is how to log into the CSE 15L account on ieng6:  
1. **Install the code editor** [`VScode`](https://code.visualstudio.com/)  
[Click here to see what it should look like when you install VScode!](https://1drv.ms/u/s!Ansq7KSJulGthVrmNN23q1gkqqqW?e=PSTd5Y)   
Description: VScode is an offline editor that is essential in providing quick updates made to your code. After I installed the code editor, 
I went to the top-right corner and selected: File > New File. This action creates a file for you to write your code in.  

2. **Connect Remotely** by writing your account details in the terminal. Assuming it is your first time connecting to the server:  
type: **ssh cs15lsp22zz@ieng6.ucsd.edu**. Make sure to replace the `zz` with the actual letters of your account. A question regarding a  
fingerprint may pop up, so click `yes`. After this, you will be prompted to enter your password. **NOTE**: you will not be able to see  
your password when you enter it, as the password is encrypted for security. If you followed the steps correctly, [`this is what you should see`](https://1drv.ms/u/s!Ansq7KSJulGthVv9-FbGULLiOACg?e=QdtR3b)  
Description: Connecting to the server will allow you to run commands to play with the files within the server, as seen in further steps.  


3. **Run some commands!**: There are various commands that you can run in the terminal to see information about your files, such as:  
-cd ~  
-cd  
-ls -lat  
-ls -a  
[`For My Example`](https://1drv.ms/u/s!Ansq7KSJulGthWiLZn07M1DQd_Si?e=zUIp4v), I tried the command ls -lat, and look what popped up!  
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
log in with **ssh cs15lsp22zz@ieng6.ucsd.edu** again, and then type `ls` [`This is what you should see!`](https://1drv.ms/u/s!Ansq7KSJulGthWkyWHxbD9CWkx6B?e=YbOc0r)  
Description: I created a file to transfer from my computer to a remote server using scp. It was a similar process as the beginning steps, as I had to log in to the ssh account again!  

5. **Setting an SSH Key**: the ssh-keygen command creates a public key and private key; saving the hassle of needing to keep logging in to the ssh account within the terminal! In the terminal, type: `ssh-keygen OR ssh-keygen -t ed25519`. You will see it says: Enter file in which to save the key  
(/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa. Replace <user-name> with the username on your computer, and click enter twice for the two prompts that pop up after such action. [`This is what you should see after following each step!`](https://1drv.ms/u/s!Ansq7KSJulGthWp5qjU_n3O3btqO?e=nZi72E)  
  
6. **Optimize Remote Running**: Found ways to run commands in the terminal more efficiently! Saves time and the number of writing needed for a command to run!  
  [`An example of optimization can be seen here`](https://1drv.ms/u/s!Ansq7KSJulGthWw7k9wsBD3Uu7BG?e=usfg7D)  
