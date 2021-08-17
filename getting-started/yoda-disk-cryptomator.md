# Encrypting your data using Cryptomator and CyberDuck

To work with privacy sensitive data you might be required to encrypt the data you store on Yoda. 
An easy way to do this is to use CyberDuck (or MountainDuck) together with the free tool Cryptomator. 

Cryptomator is available for Windows, MacOS and Linux.

![](screenshots/cbd-cryptomator-overview.png)

Note this workflow means local copies of the files on your laptop are not in the encrypted vault. 
To make sure local files are also safely encrypted you should enable Bitlocker, this should be the case on all VU laptops. 

# Using Cryptomator
First connect to the Yoda disk using [CyberDuck](yoda-disk-cyberduck.md).

## Install Cryptomator
 Download and install from the [Cryptomator](https://cryptomator.org/) site.

## Create a new Cryptomator vault
Right click in CyberDuck and choose "New Encrypted Vault"
![alt text](screenshots/cryptomator-create.png "Create vault")
Give the folder a name and set a passphrase.

![alt text](screenshots/cryptomator-passphrase.png "Create vault, set passphrase")
The vault will look like a normal folder in CyberDuck

![alt text](screenshots/cryptomator-folder.png "Cryptomator folder")

When you doubleclick the new folder you will be asked for the passphrase.
![alt text](screenshots/cryptomator-passphrase-prompt.png "Cryptomator folder")

Enter the correct passphrase and the folder will be opened as normal. You can now work with the vault as with a normal folder.

If you cancel the passphrase prompt you will only see the Cryptomator files in the folder. Adding or deleting files could corrupt your data!

If you are not prompted for the passphrase click refresh first.
![alt text](screenshots/cyberduck-refresh.png "Cyberduck refresh")




