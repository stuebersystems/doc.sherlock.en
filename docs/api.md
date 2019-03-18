# The CONFIRE SHERLOCK API

The CONFIRE SHERLOCK API is a DLL (Dynamic Link Libary) that can be integrated into virtually any programming environment. The API exports functions that provide the essential part of functionality to the CONFIRE SHERLOCK CONTROL from the Windows control panel.

The following integration scenarios are possible with the API:

* Programming a command line application to remotely operate CONFIRE SHERLOCK via command line. The [CONFIRE SHERLOCK CONSOLE] is an example of such a command line application.

* Programming a PowerShell cmdlet to remotely control CONFIRE SHERLOCK via PowerShell script.

* Integrating the API in Software Management System to remotely control CONFIRE SHERLOCK in the context of software distribution or control.

Reasons to remotely control CONFIRE SHERLOCK:

* Automate deactivation and reactivation of hard drive protection at a scheduled time in order to be able to install Windows Updates or other software updates.

* Automate configuration of CONFIRE SHERLOCK as part of an imaged-based reinstallation of computers in a computer workshop.

The interface description of the API is a result of the source code of CONFIRE SHERLOCK CONSOLE on [GitHub].

[CONFIRE SHERLOCK CONSOLE]: console.md
[GitHub]: https://github.com/stuebersystems/sherlock.console