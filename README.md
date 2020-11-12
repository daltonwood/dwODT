# dwODT
Config files used for installing various MS 365 applications using Microsoft's Office Deployment Tool via CLI/Run

Download the Office Deployment Tool and read documentation at https://aka.ms/ODT

# Instructions
Upon downloading and running the .exe it will ask for a folder to extract files to, ideally you should pick a network location intended for file sharing - this way users have appropriate permissions to execute these files.

Once you've picked a folder and extracted the files, drop the dwODT files in the same folder.

From CLI/Run enter the command for the app(s) you desire

Note: ODT treats this installation as your 'Office installation', meaning if you choose to install only one app then it will be treated as your entire Office installation, you cannot install another Office app without uninstalling and re-installing or by using a special standalone installer (see OneNote
