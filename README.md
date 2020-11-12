# dwODT
Configuration files used for installing various MS 365 apps using Microsoft's Office Deployment Tool via CLI/Run.

Download the Office Deployment Tool and read documentation at https://aka.ms/ODT

This configuration set offers:
* "Silent" install (black cmd window until completed)
* Standalone Office app install

# Instructions
Upon downloading and running the .exe it will ask for a folder to extract files to, ideally you should pick a network location intended for file sharing so users have appropriate permissions to execute these files.

Once you've picked a folder and extracted the files, drop the dwODT files in the same folder.

From CLI/Run enter the command for the app(s) you desire

|All apps|\\\\SERVER\SHARE\setupodt.exe /Configure BusRet64.xml|
|-|-|
|Access|\\\\SERVER\SHARE\setupodt.exe /Configure justAccess.xml|
|Excel|\\\\SERVER\SHARE\setupodt.exe /Configure justExcel.xml|
|OneNote|\\\\SERVER\SHARE\setupodt.exe /Configure justOneNote.xml|
|Outlook|\\\\SERVER\SHARE\setupodt.exe /Configure justOutlook.xml|
|Skype|\\\\SERVER\SHARE\setupodt.exe /Configure justSkype.xml|
|Teams|\\\\SERVER\SHARE\setupodt.exe /Configure justTeams.xml|
|Word|\\\\SERVER\SHARE\setupodt.exe /Configure justWord.xml|


# Notes
Please note that ODT treats the app(s) you install as your "Office installation" meaning if you only install one app it will not let you install another as you'd be "modifying your office installation". You would need to uninstall Office and re-install using the correct configuration, or simply install the entire suite.

If you need to install more than one app, but not the entire office suite, then please use ExcludeApp.xml for reference. See additional configuration options [here.](https://docs.microsoft.com/en-us/deployoffice/office-deployment-tool-configuration-options)
