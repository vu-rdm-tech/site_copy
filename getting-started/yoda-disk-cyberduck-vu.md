# Using Cyberduck with Yoda

_Brett Olivier - version 4_

Cyberduck is desktop software for Microsoft Windows 10 and Apple OSX that can be used to transfer files between your computer and Yoda. In this guide we will explain how to install Cyberduck, create a new connection (bookmark) to Yoda and end with some frequently asked questions and tips on using Cyberduck

# Getting Cyberduck

**Apple OSX** : Cyberduck can be installed from the VU software center or downloaded from the internet.

**Microsoft Windows 10** : Download Cyberduck from [https://cyberduck.io/download/](https://cyberduck.io/download/) it is free and you **do not** need to register.

![](Guide-Yoda-cyberduck-v2_html_b0cf2dec91193beb.png)

Run the downloaded installer by double clicking on "Cyberduck-installer.exe" which you will find in your Download folder in explorer. Install Cyberduck with the default options, and once that is done launch Cyberduck from the start menu.

![](Guide-Yoda-cyberduck-v2_html_1e666a242c864387.png)

# Configuring Cyberduck

## Accessing Cyberduck's settings

Cyberducks settings can be accessed by going to the Edit â preferences:

![](Guide-Yoda-cyberduck-v2_html_9c471886ff7038f2.png)

## Single threaded WebDAV copying

Before using Cyberduck you should change the following settings that ensure better data integrity and more reliable file transfers. First go to Cyberducks settings menu and Select "Transfers" from the top menu.

Make sure "Transfer Files" is set to "Open single connection" and that "Segmented downloads â¦ " is not selected (it is on by default). When using Cyberduck and webDAV it is strongly advised to use the single connection mode.

![](Guide-Yoda-cyberduck-v2_html_46a8be13d932e4.png)

**Setting single connection mode**.

Close the settings by clicking the x on the top right of the window.

#

# Create a new secure WebDAV (HTTPS) connection to Yoda (bookmark)

First create a new bookmark by pressing the + button on the lower left side of the screen.

![](Guide-Yoda-cyberduck-v2_html_5a54a02aa3855b4.png)

You will now see a new connection page:

![](Guide-Yoda-cyberduck-v2_html_df10437ef08ceef.png)

Click on the "FTP (File Transfer Protocol)" dropdown list and select a **WebDAV (HTTPS)** connection

![](Guide-Yoda-cyberduck-v2_html_153abfb13310ee0a.png)

and you will see the WebDAV (HTTPS) connection page.

![](Guide-Yoda-cyberduck-v2_html_10b7060315d6a7bc.png)

Fill in the following information in the appropriate blocks

- Server: **data.yoda.vu.nl**
- Username: your vunet-id (abc123)
- Password: (optional) if you don't fill this, recommended for data security, you will be asked to do so when you connect.

Cyberduck uses your home folder as a default directory to download files. This can be changed by clicking on "More Options" and choosing a new folder

![](Guide-Yoda-cyberduck-v2_html_a813126402b389cb.png)

You have successfully created a bookmark, close the editing window by clicking on the R X button on the top right of the edit window to return to the main Cyberduck screen.

# Connecting to Yoda

The main screen shows all the connections (bookmarks) you have defined. To connect, double click on the bookmark (in this case "data.yoda.vu.nl - WebDAV (HTTPS)") and you will be connected.

![](Guide-Yoda-cyberduck-v2_html_f9a0cf734c063d8d.png)

If you did not fill in your password in the bookmark you will be asked to do so now. Please note, "Save password" is automatically selected by Cyberduck, you may decide to (un)check this option. Fill in your vunet-id password and click " **Login**" to connect.

![](Guide-Yoda-cyberduck-v2_html_6f0137a7241dfc21.png)

You should now see your project directory in an explorer like window:

![](Guide-Yoda-cyberduck-v2_html_9b041059c4318bdf.png)

# Working with Yoda folders and uploading/downloading files

Click on a \> to open a folder,

![](Guide-Yoda-cyberduck-v2_html_b9a4c6811cf6a7ab.png)

or double click to open in the main window.

![](Guide-Yoda-cyberduck-v2_html_2a49a2a6c1dcb806.png)

Use the left, right and up arrows to navigate the directory tree and right click on the main window to create a new folder:

![](Guide-Yoda-cyberduck-v2_html_c51ad1193bd564da.png)

Alternatively, drag-and-drop folders and files from Windows Explorer to your Yoda project folders:

![](Guide-Yoda-cyberduck-v2_html_32a48e43b6c215fa.png)

In either case, once copying has started you should see the transfer window. Keep this open until the transfer is complete. ![](Guide-Yoda-cyberduck-v2_html_bc1b40e2f7d9db03.png)

![](Guide-Yoda-cyberduck-v2_html_ab0b29929ada8fa2.gif)

Alternatively, the context menu (activate by right clicking on a Yoda project file/directory) has a number of options for uploading, downloading and synchronizing files and folders:

![](Guide-Yoda-cyberduck-v2_html_edf94f44cf67dbc6.png)

#

## Some things to consider when using CyberDuck/webDAV

### Total path and file length

When using Cyberduck you need to make sure that your path lengths (directories + filename) are less than 255 characters long. When using webDAV this is also true on the server side (Yoda) this includes server name, project name and project folders. Be careful when copying deep directory structures and very long filenames to Yoda using Cyberduck and webDAV. Fortunately, Cyberduck will display an error message and not copy theile when either trying to copy a file with a too long source or destination path. This error is typically "access denied" (403 or 500) error and if you click "continue" CyberDuck simply skips that file and it is not transferred to Yoda.

# Recommendation. If you get "access denied errors" when transferring files with Cyberduck:

-
# Make a note of which files fail to copy.
-
# Flatten the directory structure or shorten the filename.
-
# Zip the "main" directory branch(es) that contain the long path names into individual ZIP archives.

# Frequently asked questions

## Q1) When I try to delete a file, I get a "cannot delete \<filename\>" Cyberduck error.

![](Guide-Yoda-cyberduck-v2_html_b3ce5de464c3b1e8.png)

This error message can appear when the file/folder is read-only. Read only access can be a result of:

- The folder has been locked.
- You have been given read-only access to the project folder

_Answer: unlock the folder in the research portal or get project read/write access._

## Q2) I copy a file using Cyberduck, the transfer succeeds but I don't see the file in the portal.

The folder you are copying to is marked as read only. Read only access can be a result of:

- The folder has been locked in the Yoda portal
- You have been given read-only access to the project folder

_Answer: unlock the folder in the research portal or get project read/write access._

## Q3) I tried to delete a file but get an "Access denied" error message

One possibility is that the file has been corrupted during upload and is incorrectly registered in the iRODS database.

_Answer: Contact your data manager or iRODS administrator to fix the problem. Set Cyberduck to use single threaded WebDAV copying (See Appendix 1)_

# Cyberduck settings and functionality

# Configuring Cyberduck

## Accessing Cyberduck's settings

Cyberducks settings can be accessed by going to the Edit â preferences:

![](Guide-Yoda-cyberduck-v2_html_9c471886ff7038f2.png)

## Enabling checksum verification

Cyberduck can try to verify that a file was downloaded or uploaded using an internal checksum. To enable this functionality, first go to Cyberducks settings menu and Select "Transfers" from the top menu and the "Checksum" tab. Enable the upload/download verification as required. Enabling either of these options can **negatively** affect Cyberduck's file transfer performance, however, the **upload** option is highly recommended for ensuring **archive** data integrity.

![](Guide-Yoda-cyberduck-v2_html_804e82bfe51f7521.png)

Close the preferences window to save your new configuration.

## Protecting your Yoda files with Cyberduck and CryptoMator

If you need to store encrypted files and directories on Yoda this can easily be done using Cyberduck and the client-side encryption tool CryptoMator ([https://cryptomator.org/](https://cryptomator.org/)). Working securely with data includes protecting remote/cloud data, protecting data when it is transferred from the client to the server and protecting the data on your local hard disk.

![](Guide-Yoda-cyberduck-v2_html_159cdd311b1dd82f.gif)

In the above figure we see how Cyberduck/CryptoMator can be used with Yoda. Note, we assume your local/laptop drive is protected with Bitlocker or equivalent disk encryption.

For more information see the Yoda help pages or contact the RDM support desk [rdm](mailto:rdm@vu.nl)[@vu.nl](mailto:rdm@vu.nl) (C) Vrije Universiteit Amsterdam 2021 licensed as CC-BY 4.0
