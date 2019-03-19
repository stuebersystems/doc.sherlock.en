![Build status](https://ci.appveyor.com/api/projects/status/t0s34bkrdwvc9ouh?svg=true)

# CONFIRE SHERLOCK Documentation

This is the English documentation for [CONFIRE SHERLOCK](https://sherlock.stueber.co.uk). The documentation is Open Source and we have implemented it using [MkDocs](https://www.mkdocs.org) and [Material for MkDocs](https://squidfunk.github.io/mkdocs-material). Push-Requests in the master-branch are triggered in [AppVeyor](https://www.appveyor.com) so that each change is published automatically.

## Install MkDocs for Windows

1. Install [Python](https://www.python.org). Go to the [Python downloads page](https://www.python.org/downloads/) and download the latest version for Windows. For example, for Version 3.7.2 this would be the link: [Windows x86-64 executable installer](https://www.python.org/ftp/python/3.7.2/python-3.7.2-amd64.exe).

2. Launch the installer and follow the on-screen instructions.

3. Run the command prompt as Administrator.

4. Enter the command `python --version` and `pip --version` to check the Python installation. In both cases a version number should appear as an output in the command prompt.

5. Enter the command `pip install mkdocs` to insteall the Python-Package MkDocs.

6. Final test: Enter the command `mkdocs --version`. A version nummer in the command prompt will let you know if everything has been installed correctly.

## Clone Repository

This repository is a Git-Repository. To clone the repository on a local commputer you will need a Git client. Either install [Git for Windows](https://gitforwindows.org/) and use the command prompt or install one of the many GUIs. We recommend [GitHub Desktop](https://desktop.github.com) or [SourceTree](https://www.sourcetreeapp.com).

1. Create a local directory for the documentation e.g. `c:\docs\sherlock`.

2. Open the command prompt and change to directory `c:\docs\sherlock`.

3. Enter the command `git clone https://github.com/stuebersystems/doc.sherlock.de.git` to clone the repository.

## Download Repository as Zip Archive

If you don't want to use Git you can even download the repository as Zip Archive:

1. Open the URL `https://github.com/stuebersystems/doc.sherlock.de` in your web browser

2. Click on the `Clone or download` button then select `Download ZIP`.

3. Exract the Zip Archive to any local folder, e.g. `c:\docs\sherlock`.

##  Using MkDocs

You have installed Python and the MkDocs package, you have cloned this repository or downloaded as a Zip Archive. Now you can generate the documentation locally on your computer:

1. Start the command prompt and change to the directory `c:\docs\sherlock`.

2. Enter the command `mkdocs build`. CONFIRE SHERLOCK Dokumentation will be regenerated.

3. To display the result, enter the command `mkdocs serve` and open the URL `http://127.0.0.1:8000` in your Web browser.

The table of contents can be found in the `mkdocs.yml` file and the individual chapters are in the `docs` subdirectory. 

## Further Informationen

+ [Git - All you need to know](https://git-scm.com/book/de/v2)
+ [MkDocs Overview](https://www.mkdocs.org/#overview)

## Can I help?

Yes, that would be much appreciated. The best way to help is to post a response via the Issue Tracker and/or submit corrections via a Pull Request.

## Code of Conduct

The [STÜBER SYSTEMS Code of Conduct](https://www.stueber.co.uk/code-of-conduct.php) was adopted in this project.
