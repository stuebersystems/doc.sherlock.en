# Tips & Tricks

## Partition Your Computers

A computer generally has one or more hard drives. Each one of these hard drives can be logically divided into partitions. It’s common to divide a computer into two or three partitions. The first partition is nearly always the system partition as in the one where the operation system is installed on. Some computers possess just a single partition.

If you would like to protect all partitions that’s no problem. However, if you would like to only partly protect your computers, this opens up other possibilities such as saving files permanently on for instance a D (data) partition and using CONFIRE SHERLOCK to protect the C (system) partition. In this way the computer gets the stability of an unchanged system drive and the users get the flexibility of permanent data.

An alternaitve and often even more efficient possibility to permanently save files is to set up a personal folder for each user in the network. The advantage of this approach is of course that the folder does not need to be located on a local folder and is not subject to risky hardware failure.

## The Computer’s BIOS

CONFIRE SHERLOCK offers the possibility to comprehensively protect your computers. As an extension of the operating system CONFIRE SHERLOCK can only work effectively when the operating system is running. On each computer at the end of the start-up process the operating system is launched and executed. This start-up process is initialized by the so-called BIOS (Basic Input Output System), a small specialized piece of software which is saved on the motherboard. This BIOS allows its configuration to be changed and with it certain behaviours of the computer. This is the only way someone could attempt to bypass the protection of CONFIRE SHERLOCK by starting a second operating system from floppy disk or CD-RAM for example. This behaviour is obviously undesired and should therefore be prevented by you:

* Configure the so-called boot-order in the BIOS in such a way that the hard drive with the Windows operating system is always the first to be booted from. This way you can prevent an external disk of some kind to be inserted and booted from.

* Every BIOS allows you to password-protect the configuration. Use this option to prevent unauthorized access. Unfortunately some BIOS manufacturers pre-set the BIOS with a master password. That means despite best endeavors, password protection can prove impossible. Should that be an issue for you we can only recommend disabling the Windows restart and shut down options and securing the computer case, thus making the computer’s restart switch and network cable inaccessible.

## Windows Safe Mode

As your computer starts press and hold the F8 key. You will receive a selection of possible modes to start your computer in. The top option is “Safe Mode” and ensures that only basic drivers, services and programs are run. Safe mode is useful for troubleshooting problems with programs and drivers that might not start correctly or that might prevent Windows from starting correctly.

As you can probably imagine, safe mode could offer potential to circumvent the protection of CONFIRE SHERLOCK. You need not worry, CONFIRE SHERLOCK protects your computer even in safe mode. Not only that it also continues to offer protection unaffected in all other modes.

## Limitations of CONFIRE SHERLOCK

CONFIRE SHERLOCK uses the swap file principle to bypass changes in a partition. Essentially this means: all changes are written to a special file and are reread from there. As this file always has a fixed size, it automatically has an impact on the operating function of CONFIRE SHERLOCK.

The swap file takes up space on the protected partition, thus reducing its real capacity. For large minimally used partitions this is not a problem but in small or very full partitions this is however more likely. If you create for example a 2GB swap file on a partition that has only 3GB free space available it may be that the free space is used up quickly on Windows. This should be considered when sizing the swap files. CONFIRE SHERLOCK automatically proposes a suitable size value that is based on the free memory space of the partition.

If changes to the protected drive exceed the size of the swap file CONFIRE SHERLOCK cannot continue to work. In this case, the changes must be discarded through a restart of the computer or be permanently saved. Should the swap file start running low on storage capacity CONFIRE SHERLOCK will keep you informed via the system tray icon.