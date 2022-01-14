# Lab Report 1 (introduction to 15l)
by Taegyun Yoon
## Introduction
Welcome 15l students! 
Here, this page will help you on how to succesfully log on to the remote server and do fun activities there. 

## 1. Installing VScode
* To start off, we will download VScode. It is very simple! Just go google VScode and open to see this page and download it. Or follow this link: [VScode](https://code.visualstudio.com/).
![vscode](https://github.com/tag717/cse15l-lab-reports/blob/main/Screen%20Shot%202022-01-13%20at%2020.57.57.png?raw=true)

## 2.Remotely Connecting
* Look up for own account for CSE15l in: [link](https://sdacs.ucsd.edu/~icc/index.php). Input you school account informations and you will be able to find a account ID looking like `cs15lwi22zz@ieng6.ucsd.edu`. The "zz" part is different for each user (it is your special characters!).

* Then, we go back to VScod and open a terminal. Type: `ssh cs15lwi22zz@ieng6.ucsd.edu` there and press enter. 
* You will likely see a message like below. You have to say yes and press enter to continue.
> The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 

![log in](https://github.com/tag717/cse15l-lab-reports/blob/main/Screen%20Shot%202022-01-05%20at%2016.45.07.png?raw=true)
* You will see output like this when you first log in.

# 3. Trying Some Commands
These are some codes you could try
* cd ~
* cd
* ls 
* pwd

Try it and see what it does. 
* Hint: try Ctrl-D or run the command exit to log out of the remote server.

* Mine looked like this ![example](https://github.com/tag717/cse15l-lab-reports/blob/main/Screen%20Shot%202022-01-13%20at%2023.22.28.png?raw=true)

# 4. Moving Files with "scp"

* First, create a file in VScode called whereAmI.java . It should look something like this.

> class WhereAmI{
        public static void main(String[] args){
            System.out.println("hello world!");
        }
}

* Then, type
> scp WhereAmI.java cs15lwi22zz@ieng6.ucsd.edu:~/ 

* The output will require you to enter a password. 

* Then, log into ieng6 with ssh with the use of `ls`. You should see the WhereAmI file in your directory. Now try running it by javac and java.

* Mine looked like this ![example2](https://raw.githubusercontent.com/tag717/cse15l-lab-reports/e3c24401dbf2d344755b28c565af71b54cff2d56/Screen%20Shot%202022-01-05%20at%2017.32.31.png)


# 5. Setting an SSH key
* If you think that typing password is frustrating, this is your chapter! 
* Type ssh-keygen
* If Windows, follow these extra steps [here](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation).
* This creates the private key (in `id_rsa` ) and public key (in `id_rsa.pub`). Copy the public key to the directory.
* Example of mine ![example3](https://raw.githubusercontent.com/tag717/cse15l-lab-reports/2d031e08010f34a91ce4b69402a2a049ee4cf5ff/Screen%20Shot%202022-01-13%20at%2023.55.28.png)
# 6. Optimizing Remote Running
* Write command in quotes at the end of ssh command!
* Use semicolons to run multiple commands on the same line. 
* ![example4](https://raw.githubusercontent.com/tag717/cse15l-lab-reports/1824b889c33fe749be6167ea34b1e9c24bec08ec/Screen%20Shot%202022-01-14%20at%200.32.36.png)