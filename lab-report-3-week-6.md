# Lab Report 3
## Streamlining ssh Configuration

The first step in setting up ssh configuration was to create a config file in the ssh folder. I decided to use VS Code to do this. I first opened the .ssh folder in VS Code: 

![folder](ssh-folder.png)

Then, I created a new file named config, with no file extension: 

![config](config-file.png)

To this file, I added the Host, HostName, and User information. The word after host is the alias that can be typed in the place of the full name. The HostName specifies the server, in this case ieng6, and the User is my specific username: 

![config-contents](config-contents.png)

Once this file was added and saved, I was able to ssh into my account in the terminal using only `ssh ieng6` instead of `ssh cs15lwi22arm@ieng6.ucsd.edu`. This is helpful since it is much shorter, reducing the time it takes to type, and is easier to remember:
 
![ssh](ssh-ieng6.png)

I also tried copying over a file using scp. In this case, instead of having to type out the path for the file as `cs15lwi22arm@ieng6.ucsd.edu:~/`, I was simply able to type `ieng6:~/` to copy the file, which once again is much faster and easier: 
![scp](scp-ieng6.png)