# Known bugs and workarounds

### - Special Characters (space): a space in folder names prevent the accessibility of a metadata form
If a folder path contains a space (e.g. `research-ub-test/dataset1/first experiment`), clicking on the metadata button in that folder leads to a "Page not Found" error.

A fix of this bug is waiting to be deployed on the VU Yoda, expected March 2024.

Workaround: rename the folder so it does not contain spaces, for example by subsituting with hyphens "-" or underscores "_".

Please note avoiding spaces and other special characters (e.g.: ``~!@#$%^&*()+"';:=/\<>{}`?![]|``) in file and folder names is best practice. Although Yoda allows the use of special characters they are often interpreted differently across file systems, possibly leading to issues for future users of your dataset.

### - As Group Manager: Error when trying to remove user in the Group Manager
When trying to remove a user -who has not accepted the invitation to the corresponding SRAM CO- from a Yoda group. The following error is shown:

"Something went wrong getting the unique user id for user {email}#vu from SRAM. Please contact a system administrator."

Please ignore this message: the user will still be removed from the Group and will no longer have access to the data. When you refresh the page you will see the user is no longer a member of the group.

# Recently fixed

### - Publication: Clicking on a DOI of a new published dataset leads to a "Page not Found" error. 
_Fixed 2024-02-28_


