# Known bugs and workarounds

### - Publication: Clicking on a DOI of a new published dataset leads to a "Page not Found" error
We are working with SURF to fix this bug. If possible defer submitting a dataset for publication until the bug is fixed. 

If time is of the essence please let us know via your data steward so we can prioritize fixing your dataset DOI.

### - Special Characters (space): a space in folder names prevent the accessibility of a metadata form
If a folder path contains a space (e.g. `research-ub-test/dataset1/first experiment`), clicking on the metadata button in that folder leads to a "Page not Found" error.

A fix of this bug is waiting to be deployed on the VU Yoda, expected March 2024.

Workaround: rename the folder so it does not contain spaces, for example by subsituting with hyphens "-" or underscores "_".

Please note avoiding spaces and other special characters (e.g.: ``~!@#$%^&*()+"';:=/\<>{}`?![]|``) in file and folder names is best practice. Although Yoda allows the use of special characters they are often interpreted differently across file systems, possibly leading to issues for future users of your dataset.
