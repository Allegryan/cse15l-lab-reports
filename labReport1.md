# **Lab Report 1: Remote Access and FileSystem (Week 1)**
## **Introduction**
In this lab, we'll be taking a look into the process of logging into a course-specific account on **ieng6** using Visual Studio Code and the concept of Remote Access.

## **Step 1: Installing Visual Studio Code**
To install VSCode, you'll first need to go to the following website found [here](https://code.visualstudio.com/) and follow the instructions based on your current operating system (i.e. Windows, Mac, Linux) 
![image](https://user-images.githubusercontent.com/130011927/230754839-b0ef7857-425a-44a3-a573-8c6631daab65.png)

When installed, you should be able to open VSCode and see the following screen:
![image](https://user-images.githubusercontent.com/130011927/230754890-1fdd70f0-4f76-48b3-93a1-aacaf2953e9b.png)

## **Step 2: Remotely Connecting**
For this process, you'll first need to install Git, which will provide a set of necessary tools for this step. 
Here, for example is the [link for the Windows installation for Git](https://gitforwindows.org/index.html). 
After downloading and installing, make sure to follow [these steps for utilizing git bash as your default terminal on VSCode](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994).

With this setup complete, we can now go into the actual process of connecting remotely with a course-specific account on ieng6.

In the context of CSE15L, you'll want to type the following command in the terminal (which is opened by looking to the top left of VSCode and navigating to Terminal --> New Terminal):

`ssh cs15lsp23zz@ieng6.ucsd.edu`

**(Make sure that the "zz" in the example above is replaced with *your* account's specific last 2 digits !!)**

If it is your first time connecting to a certain server, you'll likely receive a message asking whether or not you'd like to continue connecting. In this case, just type `yes` in the terminal and press enter. 

Following this, you'll now be prompted to type in the password associated with your class-specific account. If you do not already know your password or would like to reset it before finishing connecting, then you can follow the steps found [here](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view).

With your account details now put in, your terminal should look something like this:
![image](https://user-images.githubusercontent.com/130011927/230755729-af571e6f-dd05-4bf2-a41c-419ab6ccbcf9.png)

And with that, your computer (*the client*) is now connected with a different computer (*the server*)! 

## **Step 3: Trying Some Commands**
Now that you've gained access to the server, you can now go ahead and test some commands that help navigate through files, directories, and paths!
Here are some examples of utilizing commands such as `ls` in the terminal:
![image](https://user-images.githubusercontent.com/130011927/230757306-11cd9034-cfc0-4bf3-b549-46e486f8e794.png)
