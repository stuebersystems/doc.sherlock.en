# The CONFIRE SHERLOCK CONSOLE

The CONFIRE SHERLOCK CONSOLE is a command line application which is included in all installations of CONFIRE SHERLOCK. The CONFIRE SHERLOCK CONSOLE can for example be deployed in the framework of admninistrative scripts in order to remotely control CONFIRE SHERLOCK. In addition, the CONFIRE SHERLOCK CONSOLE is Open Source i.e. the entire source code is hosted on [GitHub] and also serves as technical documentation of the [CONFIRE SHERLOCK API].

To start the CONFIRE SHERLOCK CONSOLE open the Windows command line and enter:

```
cfs <command> [<parameters>...]
```

A series of commands will prompt for input of an API token as a parameter. An API token is a key which is generated from the administrator password and can be obtained in CONFIRE SHERLOCK Control.

1. Open the CONFIRE SHERLOCK Control.
2. Select the “Passwords” tab.
3. Click on the API-Token button.

The following commands are available:

## set-licenseInfo

```
set-licenseInfo <User name> <User site> <Key>
```

Imports a new license. `User name` is the username, `User site` the location and `Key` the license key.

```
cfs set-licenseInfo "My Institution" "Berlin" a8abcba1ee5aa9130ff6eade72855dbd90721bf1
```

## set-licenseInfoFromFile

```
set-licenseInfoFromFile <File name>
```

Imports a new licence from a file. `File name` is the path to the license file.

Example:
```
cfs set-licenseInfoFromFile "c:\Downloads\ConfireSherlock3.lic"
```

## get-protectionMode

```
get-protectionMode
```

Outputs the current protection status of CONFIRE SERHLOCK. This command has no parameters.

Example:

```
cfs get-protectionMode
```

## set-protectionMode

```
set-protectionMode {Off|On} <Api-Token>
```

Activates and deactivates CONFIRE SHERLOCK protection.

Example (Turn on protection):

```
cfs set-protectionMode On a8abcba1ee5aa9130ff6eade72855dbd90721bf1
```

## set-adminPassword

```
set-adminPassword <New password> <Api-Token>
```

Resets the administrator password. Warning: This command results in a change of the API token.

Example:

```
cfs set-adminPassword "admin!1234" a8abcba1ee5aa9130ff6eade72855dbd90721bf1
```

## set-userPassword

```
set-userPassword <New password> <Api-Token>
```

Resets the user password.

Example:

```
cfs set-userPassword "user!1234" a8abcba1ee5aa9130ff6eade72855dbd90721bf1
```

## get-config

```
get-config
```

Returns the current configuration of CONFIRE SHERLOCK.

Example:

```
cfs get-config
```

## set-bootMode

```
set-bootMode {DiscardChanges|KeepChanges|Inherited} <Api-Token>
```

Configures boot mode.

```
cfs set-bootMode KeepChanges FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-manualOperations

```
set-manualOperations {None|DiscardChanges|ApplyChanges} <Api-Token>
```

Configures the allowed manual operations of the user.

Example:

```
cfs set-manualOperations DiscardChanges FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-autoDiscardTime

```
set-autoDiscardTime <Time> <Api-Token>
```

Configures the time of day to automatically discard changes.

Example:

```
cfs set-autoDiscardTime 12:00 FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-autoDiscardWeekdays

```
set-autoDiscardWeekdays {Everyday|{Sun,Mon,Tue,Wed,Thu,Fri,Sat}} <Api-Token>
```

Configures the days of the week to discard changes.

Example:

```
cfs set-autoDiscardWeekdays Everyday FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-hideConfigCommand

```
set-hideConfigCommand {false|true} <Api-Token>
```

Configures whether the `Changes settings` command should be hidden.

Example:

```
cfs set-hideConfigCommand false FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-hideRebootCommand

```
set-hideRebootCommand {false|true} <Api-Token>
```

Configures whether the `Restart` command should be hidden.

Example:

```
cfs set-hideRebootCommand false FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-showTrayIcon

```
set-showTrayIcon {false|true} <Api-Token>
```

Configures whether the CONFIRE SHERLOCK icon in the system tray should be displayed.

Example:

```
cfs set-showTrayIcon true FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-removableVolumesAccessMode

```
set-removableVolumesAccessMode {ReadWrite|ReadOnly|Invisible} <Api-Token>
```

Sets the standard mode for external drives.

Example:

```
cfs set-removableVolumesAccessMode ReadWrite FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-fixedVolumeProtectionMode

```
set-fixedVolumeProtectionMode <Device name> <Off|On > <Api-Token>
```

Sets the protection mode of a hard drive partition. `Device name` is the name of the drive. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs set-fixedVolumeProtectionMode \Device\HarddiskVolume2 On FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-fixedVolumeBootMode

```
set-fixedVolumeBootMode <Device name> {DiscardChanges|KeepChanges|Inherited} <Api-Token>
```

Sets the default behaviour when restarting a hard drive partition. `Device name` is the name of the drive. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs set-fixedVolumeBootMode \Device\HarddiskVolume2 DiscardChanges FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-fixedVolumeBootAction

```
set-fixedVolumeBootAction <Device name> {NoAction|DiscardChanges|ApplyChanges} <Api-Token>
```

Sets the default behaviour when restarting a hard drive partition. `Device name` is the name of the drive. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs set-fixedVolumeBootAction \Device\HarddiskVolume2 DiscardChanges FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

set-fixedVolumeManualOperations

```
set-fixedVolumeManualOperations <Device name> {None|{DiscardChanges,ApplyChanges}}  <Api-Token>
```

Sets the allowed manual operations of a hard drive partition. `Device name` is the name of the drive. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs set-fixedVolumeManualOperations \Device\HarddiskVolume2 DiscardChanges FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-fixedVolumeAutoDiscardTime

```
set-fixedVolumeAutoDiscardTime <Device name> <Time> <Api-Token>
```

Sets the time of day to automatically discard changes of a hard drive partition. `Device name` is the name of the drive. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs set-fixedVolumeAutoDiscardTime \Device\HarddiskVolume2 12:00 FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-fixedVolumeAutoDiscardWeekdays

```
set-fixedVolumeAutoDiscardWeekdays <Device name> {Everyday|{Sun,Mon,Tue,Wed,Thu,Fri,Sat}} <Api-Token>
```

Sets the days of the weekend to automatically changes of a hard drive partition. `Device name` is the name of the drive. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs set-fixedVolumeAutoDiscardWeekdays \Device\HarddiskVolume2 Mon,Wed,Fri FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## set-removableVolumeAccessMode

```
set-removableVolumeAccessMode <Device name> {ReadWrite|ReadOnly|Invisible|Inherited} <Api-Token>
```

Sets the access mode for an external drive. `Device name is the name of the drive. You can get the list of possible names by calling *get-removableVolumes*.

Example:

```
cfs set-removableVolumeAccessMode \Device\HarddiskVolume2 Invisible FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## get-fixedVolumes

```
get-fixedVolumes
```

Returns the list of hard drive partitions.

Example:

```
cfs get-fixedVolumes
```

## get-removableVolumes

```
get-removableVolumes
```

Returns the list of external drives.

Example:

```
cfs get-removableVolumes
```

## allocate-swapStorage

```
allocate-swapStorage <Device name> <Swap size in MB> <Api-Token>
```

Generates a new swap-file for a hard drive partition. `Device name` is the name of the partition. You can get the list of possible names by calling *get-fixedVolumes*. `Swap size in MB` is the size of the swap-file in MB (Megabytes).

Example (Generate a 512 MB swap-file):

```
cfs allocate-swapStorage \Device\HarddiskVolume2 512 FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## remove-swapStorage

```
remove-swapStorage <Device name> <Api-Token>
```

Deletes the swap-file of a hard drive parition. `Device name` is the name of the partition. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs remove-swapStorage \Device\HarddiskVolume2 FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## remove-swapStorages

```
remove-swapStorages <Api-Token>
```

Deletes all swap-files.

Example:

```
cfs remove-swapStorages FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
```

## get-swapStorageInfo

```
get-swapStorageInfo <Device name>
```

Displays info of a hard drive partitionition. `Device name` is the name of the partition. You can get the list of possible names by calling *get-fixedVolumes*.

Example:

```
cfs get-swapStorageInfo \Device\HarddiskVolume2
```

## prepare-system

```
prepare-system <Api-Token>
```

Prepares the local computer so that activation of protection under ideal requirements can take place. This command should be called immediately before the system is restarted if the previous protection was activated using *set-proctectionMode*.

Example:

```
cfs prepare-system FE520676B1A1D933674F3632EAEEB163D1E88244F5EB1DEDABAB2319EEA010EB
``` 

[GitHub]: https://github.com/stuebersystems/sherlock.console
[CONFIRE SHERLOCK API]: api.md