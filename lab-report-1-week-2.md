# How To Access Your ieng6 Account 
## Step 1 - Installing VS Code
The first step is to install a text editor in order to write and edit your code. In this case, the editor that I am going to use is Visual Studio Code. In order to install it, I just Googled "Visual Studio Code" in my browser, bringing up the following page: 

![Image](vs-code.png)

From here, click download and follow the instructions to get VS Code set up on your computer. 

## Step 2 - Connecting Remotely
The next step is to set up a remote connection. Before using a course-specific account for the first time, you will need to change the account password at [Password Change](https://sdacs.ucsd.edu/~icc/index.php). This takes around 15 minutes to reset. 

Since I am on a Windows computer, I also had to install OpenSSH. This can be done from settings, going to Apps, then Optional Features. Search for OpenSSH and install, as shown below:

![Image](openssh-install-updated.png)

Now, you can open a new terminal in VS Code, and to log in remotely, use the `ssh` command, followed by the course specific account. Once this is entered, the terminal will prompt you to enter your password. You should then be logged in to the server: 

![Image](remote.png)

## Step 3 - Trying Out Commands
Now that you can access the remote server, the next step is to be able to use the terminal to execute actions using commands. Some common commands and their uses are:
- `ls` : shows you the contents of the directory you are currently in
- `cd` : allows you to change your directory
- `ls -a` : shows you all the contents of the folder, including hidden files
- `pwd` : prints the path name of the directory you are in
- `exit` : logs out of the server and returns to the local terminal

Here is an example of running some of these commands:

![image](commands.png)

## Step 4 - scp Command: Moving Files


## Step 5 - Setting an SSH Key

## Step 6 - Optimizing Remote Running