---
title: "Getting Chummy with Terminal"
layout: splash
---

# Getting Chummy with Terminal

If you are in the IT industry, and you are going to be dealing with computers and servers, you can't run away from the terminal. In fact the terminal should be your best friend. The terminal provides direct access to the computer's underlying file system and low-level features, allowing you to execute complex tasks quickly and even automatically. It provides a shell, an environment, to execute shell commands and shell scripts. There are different flavours of OS, and each has their own flavour of terminal.

<img src="{{site.baseurl | prepend: site.url}}assets/images/linux_terminal.png" alt="Linux Terminal" />
_Linux Terminal_

<img src="{{site.baseurl | prepend: site.url}}assets/images/macOS_terminal.png" alt="MacOS Terminal" />
_MacOS Terminal_

<img src="{{site.baseurl | prepend: site.url}}assets/images/windows_terminal.png" alt="Windows Terminal" />
_Windows Terminal_

For the uninitiated, the windows full of jargons might seem daunting but it's actually very fun when you get the hang of it. Who doesn't like to be in command using commands? While the different OS has their own type of terminals, the concept of how to interact with the terminal is largely the same. All of them follows a hierachical file system, which you should be familiar with in the form of a graphical interface where you navigate with a cursor. In the terminal, you navigate through the different folders and levels using commands, using the Command Line Interface(CLI). Those who are interested in working in an IT role, start with learning to use the terminal on Linux. 

----------------------------------------------------------------------------------------------------

If you are clueless about what I have mentioned, fire up your terminal and get a feel of it. Follow along with me in the following example. I will be using the linux terminal. For those using MacOS, it is Unix based, so the commands will be largely the same. For windows users, open up powershell and I include the corresponding commands in the example in brackets if it is different.

I learned to use the terminal by just typing away and making mistakes, and then there was lots of google. Almost everything can be found on google, so if you don't know how to open up your terminal, try clicking around or just google.

Now that you have your terminal ready. I hope this short exercise can give you a jumpstart in navigating the terminal.

First command, type `pwd` to show the present directory(location or folder) that you are in.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/1.png" alt="" />

Next, type `ls` to list out all the files in the current directory.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/2.png" alt="" />

You can add a switch as follows, to modify the command. Switches gives you more control over what you want to execute. In this case, `-l` organises the items in the directory into a nice list for you to look at. (For powershell, `ls` is already organised in the list format, so there is no `-l` switch.)
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/3.png" alt="" />

Next, type `cd Documents/`. The `cd` command allows you to change directory and navigate to other folders.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/4.png" alt="" />

Now that you are in the Documents folder, make a new folder using `mkdir (name of folder)`.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/5.png" alt="" />

`cd` to the folder that you have just created.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/6.png" alt="" />

Create an empty text file using `touch (filename.txt)`
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/14.png" alt="" />

Open up the text file using `nano (filename.txt)`. (For powershell, use `notepad (filename.txt)` to open the file in notepad.)
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/15.png" alt="" />
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/7.png" alt="" />

Enter anything you want in the editor, then press `crtl-X` or `cmd-X` to exit and save the file. (or as you would when using notepad)
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/8.png" alt="" />
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/9.png" alt="" />

Back to the terminal, use the command `cat (filename.txt)` and the contents that you have just entered into the text file will be printed on the terminal.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/10.png" alt="" />

Now, use `cd ../..` to go back up 2 levels in the directory. Each `..` is 1 level.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/11.png" alt="" />

And you can use `pwd` to check which directory you are in now.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/12.png" alt="" />

Now try to navigate back to the folder you created earlier and see if your text file is there.
<img src="{{site.baseurl | prepend: site.url}}assets/images/Terminal-eg/13.png" alt="" />

That's all for this exercise. If this helped to pique your interest, go ahead, explore more by yourself and figure out the tips and tricks. In my next post, I will be sharing on picoCTF, and their practice picoGYM, where we can try out more things using the CLI.

tldr; You should get familiarised with using the terminal. An example using the terminal.
