---
title: "Learning Playground 1: PicoCTF"
layout: splash
---

picoCTF is a free, original computer security education program based on a Capture-The-Flag(CTF) framework developed by security and privacy experts at Carnegie Mellon University. Originally aimed at high school students, it has various resources that are beginner-friendly. The purpose is to help participants get hands-on experiences in a safe environment. The flags are usually a hidden string that you have to find using various techniques. 

Here, I will be sharing specifically on their picoGYM where people can practice to solve challenges from previous picoCTF competition. The challenges are categorised into different areas such as cryptography, forensics, web exploitation and etc. Each challenge has varying difficulty level and scores tagged to it. You can choose to attempt the categories and levels that best suit your interest and abilities. If you are new to this, I suggest starting from the General Skills category. 

I recently started practising on their picoGYM and this is my current progress. I have completed all the general skills challenges and I am starting on other categories.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/2.png" alt="" />

Let me walk you through an example to get you started. First, head to [picoCTF](https://picoctf.org/) and go to the `Practice` tab. Scroll down and click `Practice picoGYM`.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/1.png" alt="" />

Sign up for an account. Once you are in, filter to `General Skills` and click on `Wave a flag` challenge card. A popup will show. In the challenge card, there are 3 main sections, a description of the challenge, a hints section and the flag submission section.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/3.png" alt="" />

On the side of the webpage, you can open up a `>_Webshell`. The webshell is a browser-based command line Linux environment with many common tools pre-installed. Using the webshell is not necessary for solving challenges, but it can be useful in cases where players cannot (or do not want to) install software on their machines. While many challenges can be solved with only the webshell, some may require additional tools.

Now, open up the webshell, key in your username and password.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/9.png" alt="" />

Refering back to the challenge card, this challenge is to introduce you to the help function for tools and commands. Next, take a look at hint number 2. It shows you how you can access and download the challenge file to the webshell. Copy the command shown.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/4.png" alt="" />

Head back to the webshell and paste the command you just copied.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/11.png" alt="" />

Use `ls` to see your downloaded file `warm` in the directory.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/12.png" alt="" />

Looking at hint number 3, it is telling us to change the permission for the file to be executable before running it.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/5.png" alt="" />

In the webshell, enter `chmod +x warm`. Then you can enter `ls -l` to see that the permissions for the file is now `-rwxrwxr-x`.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/13.png" alt="" />

Next, run the file by typing `./warm`. It tells us to pass `-h` to invoke the help section for the file. Now, type `./warm -h` to run the file again and you will see the help section where the flag is hidden.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/14.png" alt="" />

Copy the flag and return to the challenge card. Paste the flag into the text box and press `Submit Flag`.
<img src="{{site.baseurl | prepend: site.url}}assets/images/picoCTF/15.png" alt="" />

And there you go! You have completed a challenge. Now go ahead and try other challenges. Whenever you encounter any roadblocks, remember to check the hints and picoCTF resources. Try to use your problem solving skills. And when you are really stuck, don't be afraid to google for walkthroughs. Learn the process of how others approach the challenge. Happy capturing some flags!

tldr; picoCTF has a practice gym where you can have fun learning and practising cybersecurity.
