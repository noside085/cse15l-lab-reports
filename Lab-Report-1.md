# Lab Report 1

## Step One : VS Code

In order for us to connect remotely to servers, we must have the correct setup.
First download [Visual Studio Code](https://code.visualstudio.com/), the IDE (Integrated Developement Environment) 
that we will be using to connect to the server and run commands on. After downloading and opening the software, you
should see something similar to the image below. 

put image here

## Step Two : Account Information

After settign up VSCode, follow this [link](https://sdacs.ucsd.edu/~icc/index.php) and login by inputing your username
and PID. When successfully logged in, you should see your account lookup results, and under "Additional Accounts", 
there will be a button with your account username for remote logging. Your username should look similar to this:

`cs15lsp23xx` , where `xx` would be replaced by 2 letters, different for each person.

After clicking the button, we need to set a password in order for us to login with it. Click on the "Global Password Change Tool"
link. 

Image 2

Then procceed to the "Proceed to the Password Change Tool" link, and type in your username for the remote logging.

Image 3

Image 4

Following the instructions after typing in your username, the system should send an email to your UCSD email and from there
you would be able to change your password for your `cs15lsp23xx` account.

## Step Three : Git (Only for Windows)

Note that if you are on Mac, you are good to skip to the next step. If you are on Windows, download [Git](https://gitforwindows.org/).
After successfully downloading Git, make sure to set your terminal to Bash, following this [tutorial](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994).

## Step 4 : Connecting Remotely

Open up your terminal on VS Code by clicking on "Terminal" then "New Terminal" on the top left of VS Code. When opened, 
the terminal should be a `$`. The dollar sign indicates where you can type and the start of a new command line. In order
to login, use `ssh` as followed to login:

`$ ssh cs15lsp23xx@ieng6.ucsd.edu`

Remember to replace `xx` with the 2 letters of your own account! After inputting the `ssh` command, you will be greeted by this:

Image 5

Since this is your first time logging in, it isn't unusual to see something that confirms your actions. Continue by typing
`yes`. After doing so, the server will ask you to type in a password, which would be the one that you changed earlier. 

Hopefully, if everything went well, you will see a bunch of lines pop up, welcoming and indicating that you have logged in
successfully. 

However, in my case, not everything was smooth sailing. When logging into my `cs15lsp23xx` account, I was greeted by a bunch 
of errors instead of the Welcome message, and in order to login, I used my UCSD email username (xxxx@ucsd.edu) instead of 
the `cs15lsp23xx` in front of `@ieng6.ucsd.edu` instead.

Step 5: Running Commands Remotely

When you get to this step, you can explore a bit of the remote server by running a variety of commands. Some simple commands
that you can run are listed below:

1) `cd` -  Used for changing directories
2) `ls` - Brings up a list of files and lists in the current directory
3) `ls -a` - Brings up all entries, event the hidden ones
4) `ls -t` - Gives the time modified for entries

Image 6


