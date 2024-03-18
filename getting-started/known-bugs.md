# Known bugs and workarounds

### - As Group Manager: Error when trying to remove user in the Group Manager
When trying to remove a user -who has not accepted the invitation to the corresponding SRAM CO- from a Yoda group. The following error is shown:

"Something went wrong getting the unique user id for user {email}#vu from SRAM. Please contact a system administrator."

Please ignore this message: the user will still be removed from the Group and will no longer have access to the data. When you refresh the page you will see the user is no longer a member of the group.

### - Vault submissions fail
When a dataset submission is approved by the datamanager the data is only partially copied to the Vault space and the Status in the research space stays _Accepted_. 

Please notify us via yoda.ub@vu.nl if this happens so we can ask the system admin to restart the process manually.

The problem is under investigation at SURF.

## Recently fixed

### - Publication: Clicking on a DOI of a new published dataset leads to a "Page not Found" error. 
_Fixed 2024-02-28_

### - Special Characters (space): a space in folder names prevent the accessibility of a metadata form
_Fixed 2024-03-18_
Please note avoiding spaces and other special characters (e.g.: ``~!@#$%^&*()+"';:=/\<>{}`?![]|``) in file and folder names is best practice. Although Yoda allows the use of special characters they are often interpreted differently across file systems, possibly leading to issues for future users of your dataset.
