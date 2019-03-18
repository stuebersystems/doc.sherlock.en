# How To Get Started

## Installation

Start by visiting the [CONFIRE SHERLOCK website], and downloading the latest version of CONFIRE SHERLOCK. There are two types of installer files for CONFIRE SHERLOCK:

* `ConfireSherlockSetup64.msi` is an installer for 64bit versions of Windows.
* `ConfireSherlockSetup32.msi` is an installer for 32bit versions of Windows.

Please select the appropriate suitable installer for your operating system. If you’re not sure which is the right one for your computer just try both out. You can’t go wrong as both installers check if they are being launched on the right operating system.

To start the installation double click the installer and simply follow the on-screen instructions. At the end of the installation you will be asked to restart the computer. Please do this straight away as CONFIRE SHERLOCK installs a system driver which can only be activated once the computer has been restarted.

## Licensing

You receive a 30 day trial period in which to test out CONFIRE SHERLOCK. After this time you must decide whether to uninstall the software or acquire a license in order to use CONFIRE SHERLOCK permanently. You have to license each computer using CONFIRE SHERLOCK.

When starting CONFIRE SHERLOCK program from the Windows control panel for the first time the “Test license” dialog window will appear. This dialog window displays how many days you can continue testing CONFIRE SHERLOCK.

<figure class="center">
    <img src="/assets/images/testlicense-dialog.png" alt="The Test license dialog window">
    <figcaption>The <em>Test license</em> dialog window</figcaption>
</figure>

* If you wish to just continue using the trial click on `Start Application`.

* If you would like to use CONFIRE SHERLOCK on this computer unrestricted you will need to acquire a license from STÜBER SYSTEMS. To produce a license for you we need to know the address of your school or company as well as the number of computers you wish to enable the license for. Please use the order form for either schools or companies. You’ll then receive a license via email which can be directly imported via `Import license` or manually entered in the `Change license` dialog. You can access both of these options when either starting the application or under the "Help" tab. There just click on `Show Information`.

<figure class="center">
    <img src="/assets/images/about-dialog.png" alt="The Dialog Window About">
    <figcaption>The Dialog Window <em>About</em></figcaption>
</figure>

## Configuration

To configure CONFIRE SHERLOCK you need to open the CONFIRE SHERLOCK control panel. To open it, right click the following icon in the system tray:

<figure class="center">
    <img src="/assets/images/taskbar-red-icon.png" alt="CONFIRE SHERLOCK Protection is inactive">
    <figcaption>CONFIRE SHERLOCK Protection is inactive</figcaption>
</figure>

Select the “Change Settings” option from the pop-up menu. This will open the CONFIRE SHERLOCK control panel. Alternatively you can open CONFIRE SHERLOCK control panel from the Windows control panel.

The CONFIRE SHERLOCK control panel allows you to change the central protection off or on as well as all settings in CONFIRE SHERLOCK. Below we’ll go through the settings of each tab step by step.

On the “Start” tab you can turn CONFIRE SHERLOCK protection off and on.

<figure class="center">
    <img src="/assets/images/sysctrl-start-tab.png" alt="The Start Tab">
    <figcaption>The <em>Start</em> Tab</figcaption>
</figure>

All the computer’s hard drives and partitions are listed on the “Hard Disks” tab. For each drive you can decide whether you wish to activate protection or not. Within the list click on each of the desired drives and select the “Do protect drive” option.

<figure class="center">
    <img src="/assets/images/sysctrl-fixed-drives-tab.png" alt="The Hard Drive Tab">
    <figcaption>The <em>Hard Drive</em> Tab</figcaption>
</figure>

For each drive to be protected, you can also choose how big you want the created swap file to be. CONFIRE SHERLOCK recommends a suitable size for each swap file automatically so in most cases you won’t need to do anything. If however you would like to increase or decrease the size of the swap file click on the `Customize` button.

!!! info

	CONFIRE SHERLOCK creates a swap file for each drive to be protected. This is a special system file with an invariable size. All changes are redirected into this file before they reach the actual file system. By restarting the computer the contents of the swap file are discarded and the file system’s original data is used again.

After clicking `OK` to confirm the changes in the CONFIRE SHERLOCK control panel the swap files are automatically created. This can take a few minutes depending on the size and number of the swap files.

On the “Restart” tab you can determine the behaviour of CONFIRE SHERLOCK when restarting. You can choose whether you would like to discard all changes upon each restart or whether to do this only within specified time intervals. If going for the latter you can define an interval of weekdays and time in order to determine when the changes shall be discarded. Let’s assume you selected the weekdays Monday and Wednesday and the time 10pm. In this scenario it would apply that upon the next restart after 10pm Monday and Wednesday all changes will be wiped clean. On all other days of the week the exceedance of the time 10pm would have no effect.

<figure class="center">
    <img src="/assets/images/sysctrl-reboot-tab.png" alt="The Restart Restart Tab">
    <figcaption>The Restart <em>Restart</em> Tab</figcaption>
</figure>

If you’d like to individually configure the behaviour of each drive click on `Edit` to open the dialog window “Exceptions in the Restart Behaviour”.

Under the “External Drives” tab you will see all external drive devices which are physically connected to the computer.

<figure class="center">
    <img src="/assets/images/sysctrl-removable-drives-tab.png" alt="The External Drives Tab">
    <figcaption>The <em>External Drives</em> Tab</figcaption>
</figure>

These are for example all floppy disk drives, CD/DVD drives and USB drives. Click on any one of the desired drives and select one of the following options:

* The option “External drives have full access” means the user has unrestricted access to external drives e.g. they can read and write.

* The option “External drives are read-only” means the user has only read-only access to external drives. All write attempts are prevented.

* The option “External drives are hidden” means external drives are hidden from the user. For example, they can no longer be seen in Windows Explorer.

By default these options apply for all external drives in the system as well as future drives that are connected. You can customize the protection for specific drives under “Exceptions” by clicking on `Edit`. A dialog window will open in which you an select and customize the protection of any drive. The following options are available for each drive:

* The option “Default” means that the global configuration applies to the selected drive. The behaviour is therefore based on the settings on the tab “External drives”.

* The option “Hidden drive” mean that the user cannot see the drive in the system.

* The option “Read-only access to drive” means that the user has only read-access to the drive.

* The option “Full access to drive” means that the user has both read and write access to the drive.
* 
On the “Passwords” tab you can assign passwords with different meanings in order to protect CONFIRE SHERLOCK from unauthorized use.

<figure class="center">
    <img src="/assets/images/sysctrl-passwords-tab.png" alt="The Passwords Tab">
    <figcaption>The <em>Passwords</em> Tab</figcaption>
</figure>

<dl>
  <dt>Administrator Password</dt>
  <dd>This password prevents the CONFIRE SHERLOCK control panel from being opened. It is not possible to change CONFIRE SHERLOCK’s configuration, for example activating or deactivation protection, without knowing this password. We highly recommend that you set an administrator password.</dd>
  <dt>User Password</dt>
  <dd>This password prevents the “Reboot” menu option from being selected from the CONFIRE SHERLOCK icon in the system tray. Without knowing this password you can neither save changes permanently nor force the computer den Computer zwingen Änderungen zu einem beleibigen Zeitpunkt zu verwerfen.</dd>
</dl>

The `Show API token` button opens a dialog window which displays the current API token. The API token is a combination of letters and numbers generated from the current administrator password. It’s a kind of password which is needed in order to use the CONFIRE SHERLOCK API or CONFIRE SHERLOCK CONSOLE. Each time the administrator password is changed the API token changes too.

On the “Options” tab you can change CONFIRE SHERLOCK’s interface language and notifications and you can determine whether the system tray icon for CONFIRE SHERLOCK should be displayed or not.

<figure class="center">
    <img src="/assets/images/sysctrl-options-tab.png" alt="The Options Tab">
    <figcaption>The <em>Options</em> Tab</figcaption>
</figure>

Using the “Hide “Change settings” command” and “Hide “Reboot” command” you can affect the contents of the icon’s pop-up menu.

On the “Help” tab you can open the online help pages, display program and license information or check for a program update.

<figure class="center">
    <img src="/assets/images/sysctrl-help-tab.png" alt="The Help Tab">
    <figcaption>The <em>Help</em> Tab</figcaption>
</figure>

If you close the dialog window by clicking OK it will first check whether any new swap-files have been created. If this is the case a dialog window will appear which displays the next step of creating the files. Please note that creating a new swap-file can take several minutes depending on the size. As a rule you will be required to restart the computer. This is necessary so that the whole system can be reconfigured.

If you’ve selected the central activation on the “Start” tab CONFIRE SHERLOCK protection will be active after a restart. You will know if it’s active because the system tray icon will be green.

<figure class="center">
    <img src="/assets/images/taskbar-blue-icon.png" alt="CONFIRE SHERLOCK Protection is active">
    <figcaption>CONFIRE SHERLOCK Protection is active</figcaption>
</figure>

## Disregard Changes or Apply

If CONFIRE SHERLOCK protection is activated CONFIRE SHERLOCK will check whether the changes of the last session should be discarded, kept or applied when the computer is next restarted. You can configure this behaviour as follows:

* When you shut down the computer in the usual way using the Windows interface then the settings in the CONFIRE SHERLOCK control panel will be applied upon the next restart.

* When you right click the CONFIRE SHERLOCK system tray icon and then select “Reboot” you can overwrite the settings of the CONFIRE SHERLOCK control panel before restarting the computer.

The “Reboot System” dialog window is only available when CONFIRE SHERLOCK protection is active.

<figure class="center">
    <img src="/assets/images/userctrl-reboot-dialog.png" alt="The Reboot System dialog window">
    <figcaption>The <em>Reboot System</em> dialog window</em></figcaption>
</figure>

## Download updates

You can receive improvement updates of CONFIRE SHERLOCK. There are two ways to install an update:

* Start the CONFIRE SHERLOCK control panel and select the “Help” tab then click on “Check for updates”. CONFIRE SHERLOCK connects directly with STÜBER SYSTEMS’ internet-server and checks if a new version of CONFIRE SHERLOCK is available. If so, the installer will automatically download and open it for you.

* Should no internet connection be available on the computer that CONFIRE SHERLOCK resides on you can also download the installer on another computer and open it manually later. Please note that both reinstalls and updates are carried out by the same installer. The system detects which one should be launched.

Please also consider that an update will only effectively work when protecton is deactivated. After installing the update you will need to restart the computer for changes to take affect.

[CONFIRE SHERLOCK website]: http://sherlock.stueber.co.uk