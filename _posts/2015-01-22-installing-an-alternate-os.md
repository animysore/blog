---
published: false
---

##Why most programmers need an alternate operating system and how you should go about getting one

So, if you are reading this on a laptop or a desktop computer, I can say with 98.98 percent surety that you are using a version of either the Windows or Mac `operating system`. 

Generally, a single operating system is sufficient for most computer users. But when you are developing software for multiple operating systems, or using you're computer for things like making a web server, or running very specific development environments, often one operating system ceases to be enough.

Running more than one operating system on a computer or `dual-booting` as it is usually called ( or triple-boot, quad-boot, etc, although the word usage is not as common as dual-boot) is actually very simple and easy, but if you fail to follow some basic procedures, you could end up losing your data, or being unable to use even one OS. Even more terrible things, depending on how bad you screw up.

However operating systems need not always be *installed*. More on `Virtualization` later.

Here are some questions you will most probably have if you are new to installing operating systems : 

###1) Which OS should I install?

You should install whatever operating system best suits your particular programming requirements. Windows and OSX are generally best suited for app and software development for those platforms. For most other things, `linux` flavours are popular. If you simply want to install a linux OS, I would personally reccommend either `Ubuntu` or `Debian`. Both have easy installations, great support bases, lots of software and applications, and a modern UI. 

In the end it comes down simply to what best fits your comfort zone. The Mac OS is better suited for programming than Windows. But neither of these are as popular as open-source linux distros.

###2) Is it compulsory to install an OS to use it? 

First of all, it is not required for you to actually install an OS on your hard disk to use one. Lots of linux operating systems let you run operating systems on flash drives and cd's. Usually this is to let you demo the OS before installing, but with this method you can actually use an entire OS without it installing on your hard drive.

Almost all operating systems out there can be run by `virtualization`. What this means is that you use an os within another os. There are several great software for doing this, for both Windows and Mac (Also linux). `Virtualbox` and `VMware`(Virtualbox is free) come on the very top of the list. 

You can run pretty much any operating system - Android,iOS,Windows,OSX,(Ku/Edu/Lu/U)buntu, Debian Linux - anything as long as your processor supports (hardware)`virtualization technology` or `VT`. 

Virualbox can, to a large extent manage on older processors which do not have `VT` enabled, however performance might be low. VMware requires some bypassing commands to do the same.
{: .notice}

Anything newer than Intel `Pentium` or AMD 

###3) Are there any precautions I should take before trying to install a new OS.

**Yes!** As I mentioned before, you might murder your computer by accident when installing an OS, so always take a backup of all you data onto ANOTHER COMPUTER or a HARD DISK. 

Also its always better to partition your hard drive when you start the installation process. Most Operating Systems allow you to partition your hard drive before installation, but its always better to do it beforehand to ensure nothing goes wrong. Its usually easiest if you use your current OS to partition. If you're on Windows use the `Disk Management` tool, `Disk Utitlity` on Mac, and `GParted` on Linux.

Never,ever,ever install an OS onto the same partition as another OS. Always Take care you select an empty partition during installation.
{: .notice}