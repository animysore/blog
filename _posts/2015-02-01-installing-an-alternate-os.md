---
layout: post
title: Tips for Installing an Alternate OS
description: Why most programmers need an alternate operating system and how you should go about getting one
modified: null
tags:
  - operating
  - system
  - crosspublished
image:
  feature: "abstract-6.jpg"
comments: true
share: true
published: true
---

#### ***Why most programmers need an alternate operating system and how you should go about getting one***

![Linux Distros](/blog/images/2015-02-01-installing-an-alternate-os/linux-distros.png)

So, if you are reading this on a laptop or a desktop computer, I can say with **98.98 percent**[^1] surety that you are using a version of either the Windows or Mac `Operating System`.

Generally, a single operating system is sufficient for most computer users. But when you are developing software for multiple operating systems, or using your computer for things like making a web server, or running very specific development environments, often one operating system ceases to be enough.

Running more than one operating system on a computer or `dual-booting` as it is usually called ( or triple-boot, quad-boot, etc, although the word usage is not as common as dual-boot) is actually very simple and easy, but if you fail to follow some basic procedures, you could end up losing your data, or being unable to use even one OS. Even more terrible things, depending on how bad you mess up.

However operating systems need not always be *installed*. More on `virtualization` later.

[^1]: As according to the data shared by Netmarketshare.com

------
Here are some questions you will most probably have if you are new to installing operating systems :

### 1) Which OS should I install?

You should install whatever operating system best suits your particular programming requirements. Windows and OSX are generally best suited for app and software development for those platforms. For most other things, `Linux` flavours are popular. If you simply want to install a Linux OS, I would personally recommend either `Ubuntu` or `Debian`. Both have easy installations, great support bases, lots of software and applications, and a modern UI.

In the end it comes down simply to what best fits your comfort zone. The Mac OS is better suited for programming than Windows. But neither of these are as popular as open-source Linux distros.

### 2) Is it compulsory to install an OS to use it?

First of all, it is not required for you to actually install an OS on your hard disk to use one. Lots of Linux operating systems let you run operating systems on flash drives and cd's. Usually this is to let you demo the OS before installing, but with this method you can actually use an entire OS without it installing on your hard drive.

![Virtualbox](/blog/images/2015-02-01-installing-an-alternate-os/virtualbox.jpg)

Almost all operating systems out there can be run by `virtualization`. What this means is that you use an OS within another OS. There are several great software for doing this, for both Windows and Mac (Also Linux). **Virtualbox** and **VMware** (Virtualbox is free) come on the very top of the list.

You can run pretty much any operating system - Android, iOS, Windows, OSX, (Xu/Ku/Edu/Lu/U)buntu, Debian, Fedora, Red Hat - anything as long as your processor supports (hardware)`virtualization technology` or `VT`.

Virtualbox can, to a large extent manage on older processors which do not have `VT` enabled, however performance might be low. VMware requires some bypassing commands to do the same.
{: .notice}

Anything newer than Intel `Pentium` or AMD `Athlon` would probably support VT, but check your processor specifications before trying to run a virtual OS.

### 3) Are there any precautions I should take before trying to install a new OS.

**Yes!** As I mentioned before, you might murder your computer by accident when installing an OS, so always take a backup of all you data onto ANOTHER COMPUTER or a HARD DISK.

Before installing any OS, always read the specifications fully, including the version you are planning to install. Check on forums for any complaints people have had when they have tried to install that particular version of that OS on your computer model.

Also its always better to partition your hard drive when you start the installation process. Most Operating Systems allow you to partition your hard drive before installation, but its always better to do it beforehand to ensure nothing goes wrong. Its usually easiest if you use your current OS to partition. If you're on Windows use the `Disk Management` tool, `Disk Utility` on Mac, and `GParted` on Linux.

Never,ever,ever install an OS onto the same partition as another OS. Always take care you select an empty partition during installation.
{: .notice}

### 4) Which installation method should I use?

When you 'download an OS' in most cases you are actually downloading an `ISO` file, or a compressed `ISO` file. This `ISO` file can either be burnt to a CD, or to a USB. Its upto you, to choose which. Some old computers may not be able to boot from USB.

Its not just enough MOVING the ISO file to a CD or USB. It must be burnt, so as to make it BOOTABLE.
{: .notice}

There are plenty of software for burning ISO files. Here are two free ones, for the lazy and the uninitiated (**Disclaimer** : Don't blame me if this causes your computer to explode, or transform into a killer robot)  
   - For burning to discs : [Free Iso Burner](http://freeisoburner.com/)
   - For burning to USB : [ISO to USB](http://isotousb.com/)

![Boot Option BIOS](/blog/images/2015-02-01-installing-an-alternate-os/bios-screen.png)

After you burn the ISO image, insert the USB/Disc. Run the autorun if it has one - it most likely will - or directly proceed to restart your computer. Before your OS loads, on the BIOS screen, hit the key for the boot option menu (Usually`f9`on PC's) and select either USB or CD depending on which your OS is loaded. I bid you smooth sailing.

### 5) Precautions to take DURING installation

Stating the obvious here - Whenever you are installing a new OS, make sure to keep your computer fully charged and plugged in.

Keep your Internet easily accessible. Always. WiFi is recommended, but Cable will also work. If you use a dongle, try to convert it's  network into a hotspot as the OS you just install maybe unable to use it. Have another computer standing as backup, in case your installation goes boink.

Ensure you have all the files you may need, already downloaded and ready to be booted if required. I personally would recommend downloading the `boot repair disk` and putting it on either a bootable CD or USB, especially if you are installing Linux.

The Boot repair disk can be downloaded [**here**](http://sourceforge.net/projects/boot-repair-cd/).

The boot repair disk can be booted from directly. It's main function is to fix GRUB, but it also contains very useful tools, such as `GParted` the partition editor, as well as an `OS-Uninstaller`. It can also be used to access the Internet, in case you need some urgent help.

### 6) What should I do if something goes wrong during the install

Odds are, the install will not go *ferpectly the ristf eimt*. Maybe there were driver problems. Maybe your computer was not fully compatible with the OS version you tried to install. Maybe you made some other mistakes. Whatever happens, it's always best if you try the whole install afresh. If you think the operating system has not installed completely or with some defects, use the boot repair disk to uninstall the operating system, format the partition that you installed the OS on, and try again.

> In case of a failed install, Purge, Cleanse and Start over!

### 7) The OS has been installed. Now what?

So all the installation is done. **Check if everything is functioning as it should.** The only tests you need to run, are with the hardware. Just make sure all your hardware components - speakers, keyboard, touchpad/mouse, camera, ports - are all functioning correctly. If there is a problem with anything, try looking on forums if you're experiencing a known issue with the OS. More likely than not, the drivers will need to be updated, and once this is done, your new OS will be ready.

Also ensure your multi-boot screen is functioning correctly. ( This will be `GRUB` if you have any linux versions installed ) The boot repair disk can fix most issues with GRUB. If you have installed Windows freshly, GRUB may not be accessible during startup and you will directly boot Windows. Again, the boot repair disk can fix this issue.

![Grub](/blog/images/2015-02-01-installing-an-alternate-os/grub-screen.jpg)

> Aah, the satisfaction of using a freshly installed OS

**Some General tips for Linux :** Start using the terminal for even basic things. That way you'll get the hang of it. Install updates, as soon as you get your system up and running.

**General tips for Ubuntu :** [Click Here](http://www.unixmen.com/top-things-installing-ubuntu-14-1014-0413-1013-0412-1012-04/) for a quick list of things to do immediately after you install Ubuntu.

-----
This post is crosspublished on the [KHMD blog](http://kumaranhmd.blogspot.com)
If you found this article helpful, please Like, Comment and Share. Go forth and conquer!
