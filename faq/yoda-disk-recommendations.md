# Data transfer recommendations
Upload from laptop:
- Web portal
- WebDAV
- Rclone
- icommands

Download to laptop:
- WebDAV client
- Rclone
- irsync

To/from Yoda from a different platform 
HPC (Lisa, Bazis)
- icommands
RD
- rclone
- webdav client
SciStor
- WebDAV client
- rclone
- icommands


## Graph
TO DO: create a graph like on https://wiki.surfnet.nl/download/attachments/11219959/RD-upload-recommendations.png?version=1&modificationDate=1580395511489&api=v2

2 axis file and size
| tool | file min | file max | size min | size max |
| --- | --- | --- | --- | --- |
| portal | 0 | 100 | 0 | 5 |
| webdav client | 0 | 1000 | 0 | 100 |
| rclone | 0 | 50000 | 0 | 1000 |
| icommands | 0 | 100000 | 0 | 10000 |
| ask for help | 50000 | 1000000 | 1000 | 100000 |

## Moving data within Yoda

