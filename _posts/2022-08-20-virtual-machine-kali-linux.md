---
title: "Virtual Machine: Kali Linux"
layout: splash
---

# Virtual Machine: Kali Linux

At my current work, I deal with semiconductor machinery. The equipment that I work with usually runs on windows OS, from windows 2000 up to windows 10. And the controls for the equipment are proprietary software from the machine makers. Now, you might be thinking what has all these got to do with virtual machine(VM). First let me explain what is a virtual machine.

Based on Microsoft's definition, a VM is a computer file, typically called an image, that behaves like an actual computer. It can run in a window as a separate computing environment, often to run a different operating system—or even to function as the user's entire computer experience—as is common on many people's work computers.

Simply put, you can use a virtualisation platform, such as VMware workstation and Oracle VM VirtualBox, and load up a VM like it is another computer running with your computer. It is an environment that is separate from your host PC. This allows you to run Linux on a Windows PC, or Windows on a Mac PC and vice versa.

Going back to the equipment at my job, we use VM to train and familiarise ourselves with the equipment control software. We run the software in a VM, isolated from the actual equipment. In order to run the software in the VM without the actual equipment, the I/Os need to be disabled or dummy inputs need to be given. This is so that we do not damage or crash the equipment if we press any wrong controls. It is especially useful for training and building confidence in machine handling. Also, it can be run on any PC and there is no need to take up the equipment's precious system time for production.

That is just one small use for VM. There are so much more benefits of using a VM. For software developers, VMs allow a team to build, test, and deploy code within simulated environments without wasting computing resources. If you are in the cybersecurity field. You can create safe and isolated environment that allows you to conduct tests and analysis on malware without the risk of damaging your PC. 

In this post, I will be sharing on how to get Kali Linux on your computer. Kali Linux is a Debian-derived Linux distribution designed for digital forensics and penetration testing. It has over 600 tools for information security. It is maintained and funded by Offensive Security. And it is also free for use.

Click on [Kali Linux](https://www.kali.org/get-kali/#kali-virtual-machines) and download your preferred image for VMware or VirtualBox. After you have downloaded your file, unzip the folder.

<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/1.png" alt="" />

You will also need a virtualisation platform. Choose the appropriate one based on your host PC operating system.

[VMware Workstation 16 Player](https://customerconnect.vmware.com/en/downloads/details?downloadGroup=WKST-PLAYER-1624&productId=1039&rPId=91446)

[Oracle VirtualBox](https://www.virtualbox.org/wiki/Downloads)

For this tutorial, I will be using VMware Workstation 16 Player. For those installing on windows, just run the installer. For those using Linux for host OS, type `sh (bundle file name)` to install. If you are not in root access, use `sudo` in front.
<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/0.png" alt="" />

After you are done installing the VMware Workstation 16 Player, launch it and get through the liscense agreement.
<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/2.png" alt="" />

Once you are done, click on `Open a Virtual Machine` and browse to where you unzip the Kali Linux VM.
<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/3.png" alt="" />

Leave all the settings at default, click `Power On` and let the VM load. At the login screen, enter the default user and password which is `kali` for both.
<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/4.png" alt="" />

Now you should see the desktop interface for Kali Linux. At the top left corner there is a menu button, where you can click and see all the various information security tools categorised in their applications.
<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/6.png" alt="" />

But first things first, open up the terminal and type `sudo apt update` to get all the latest updated packages for the tools and system.
<img src="{{site.baseurl | prepend: site.url}}assets/images/VMKali/7.png" alt="" />

Now you can go ahead and explore the VM. Don't worry about breaking it because you can always do a fresh setup easily. In my next post, I will be sharing on 1 or 2 of the tools available in Kali Linux.

tldr; Virtual machine is great. I show you how to install Kali Linux.

