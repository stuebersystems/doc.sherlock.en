# Introduction

This online guide describes everything you need to know about CONFIRE SHERLOCK. We aim keep the info as compact as possible.

CONFIRE SHERLOCK protects your computers from undesired changes by users by allowing you to disregard those changes at any time. In addition, access to external drives can be limited or completely blocked in order to prevent unauthorized copying of data.

CONFIRE SHERLOCK is an efficient protection software for public computers, accessible to a large group of people and does not require any advanced system knowledge.

## Areas of Use

* Computers in training rooms
* Computers on trade show stands
* Computers in internet cafes
* Computers in the hotel lobby
* Software test labs
* Family computers at home

CONFIRE SHERLOCK protects these computers from unwanted changes and if desired also prevents data from being copied onto or taken away via USB stick.

## Highlights

* Pure software solution

* Minimal purchase costs

* Easy to use

* Minimal administration required

* Suitable for software tests

* Effective virus protection

* Supports all Windows operating systems from Windows XP to Windows 10

* An API (Application Programming Interface) allows you to manage and control CONFIRE SHERLOCK without graphical user interface.

* With the help of the CONFIRE SHERLOCK Console you can manage all settings via Windows command prompt.

!!! warning "Important note"

	CONFIRE SHERLOCK installs underneath a low-level system driver that filters access to the hard drive. This level of access to the operation system can lead to problems due to unexpected system configurations (e.g. future service packs for Windows) which despite extensive testing on CONFIRE SHERLOCK cannot completely prevented. For that reason, please take a backup of all important data and files from your computer before you begin using CONFIRE SHERLOCK. The same applies for system updates to the operating system when protection is deactivated.

As the administrator of a computer room you’re probably already aware of problems that arise from time to time when a single computer needs to be set back to its original condition because too many temporary files have built up during lessons or training courses. Or while working as the internet café administrator you don’t know which files your users have left behind, or because viruses and trojans have found their way into the system, because some important system files have been deleted, because unwanted applications have been installed. The list goes on.

One strategy that some use is to implement very strict access rights within the operating system in such a way that it hinders the user from being able to accomplish their work in any practical manner. This is in reality very impractical and time-consuming to set up (you can fill whole book shelves just on Windows security) and can very quickly lead to permission conflicts. For example, in a computer science class the students being taught may well require advanced rights to some extent in order to be able to test their software projects successfully. At the same time this opens the door for unwanted manipulations.

Another strategy might be to create and manage an image for each computer which would then have to be reloaded onto the computer each night so that all changes from the previous days can be undone. Even here the effort required is highly substantial i.e. a specialized imaging software must be obtained and a suitable network necessary to support it. This work becomes ever more increased when every time new software or update need to be installed (in this case each image must be recreated).

CONFIRE SHERLOCK opens up a third strategy which makes a simple restore of the initial state possible without having to restrict the movements of your computer users. CONFIRE SHERLOCK offers the following possibilities:

* You can undo changes on the local computer at any time. You can decide whether to restore the old state on the next restart or the next day (next week etc.).

* You can exclude individual partitions from protection. You could for example choose to protect the C: partition (i.e. the Windows operating system partition) but exclude the data partition (D: data partition) from protection. This allows a robust protection of the operating system and at the same time data can be saved and changed long-term on the second partition.

* Should you ever wish to keep changes on a protected partition permanently this isn’t a problem either. CONFIRE SHERLOCK allow you to assume these changes.

* In addition you can control access to all external drives (floppy disk drive, CD/DVD drives, USB sticks, etc.). External drives can be set to read-only or blocked entirely. If desired, you can even ensure that this drive doesn’t even appear in Windows Explorer.

* The [CONFIRE SHERLOCK API] allows you to integrate the functionality of CONFIRE SHERLOCK into your own applications. The API is a simple DLL (Dynamic Link Library) with no further dependancies.

* The [CONFIRE SHERLOCK CONSOLE] is an example for integration the CONFIRE SHERLOCK API. This command line application gives you the possibility to control/configure CONFIRE SHERLOCK via administrative scripts. For example: Automatically deactivate/reactivate the protection at a specific point in time in order to install Windows Updates.

* And last but not least: CONFIRE SHERLOCK is a pure software solution. That means you can install it on practically any computer no matter whether it’s on a laptop or a regular desktop computer.

The software is easy to install and use. You install CONFIRE SHERLOCK on each computer and configure your protection preferences.

[CONFIRE SHERLOCK API]: api.md
[CONFIRE SHERLOCK CONSOLE]: console.md