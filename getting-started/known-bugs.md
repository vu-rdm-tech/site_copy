# Known bugs and workarounds

### - Datasets can be submitted without mandatory Creator Affiliation name
When leaving the [Creator] [Affiliation Name] field empty, the system will indicate clearly that the metadata form is not complete by marking the field with a red border and showing the green "Required for the vault" bar as incomplete. 
On clicking "submit" the system should show an error "Metadata is not valid, please open metadata form for more information", but it does not and the dataset is allowed to be further processed and can be secured in the Vault normally. 
If the dataset is later submitted and approved for publication the publication process fails and no resolvable DOI is generated.

Make sure Affiliation names are added for each Creator. Note that if the institute is not in the dropdown list you can just type the Name and leave the identifier field empty.

### - As Group Manager: Error when trying to remove user in the Group Manager
When trying to remove a user -who has not accepted the invitation to the corresponding SRAM CO- from a Yoda group. The following error is shown:

"Something went wrong getting the unique user id for user {email}#vu from SRAM. Please contact a system administrator."

Please ignore this message: the user will still be removed from the Group and will no longer have access to the data. When you refresh the page you will see the user is no longer a member of the group.

## Recently fixed

### - Vault submissions fail
_Fixed 2024-05-01_
When a dataset submission is approved by the datamanager the data is only partially copied to the Vault space and the Status in the research space stays _Accepted_. 

### - Publication: Clicking on a DOI of a new published dataset leads to a "Page not Found" error. 
_Fixed 2024-02-28_

### - Special Characters (space): a space in folder names prevent the accessibility of a metadata form
_Fixed 2024-03-18_
Please note avoiding spaces and other special characters (e.g.: ``~!@#$%^&*()+"';:=/\<>{}`?![]|``) in file and folder names is best practice. Although Yoda allows the use of special characters they are often interpreted differently across file systems, possibly leading to issues for future users of your dataset.
