## How to install

First download the zip file from the following link:
![Sample1.zip](files/Sample1.zip) You can download the file anywhere on your computer and then you have to install it in VW by Opening plug-in manager from Tools->Plug-ins->Plug-in Manager and by selecting 'Third-party Plug-ins' tab and clicking Install... button. Now you have to load the zip file from the dialog. VW would first unzip the file and run install.py script if available. After restarting the VW, the two objects and one command menu is available to include in your workspace.

## How the sample works

First install.py script would look for any available .vwx and .vww files and move them to the appropriate folders.
Then the user can create a human object consisting of two separate objects named Head and Body and from the command menu can Select them all and group them as one object.
There are a couple of things to be learned from this example:

* How to write an installation script.
* How to design point objects from python
* How to traverse objects available in active layer and select them and group them from the Python script

## See Also

Python basic information: [Python](../README.md)

[Script Function Reference](../../Function%20Reference/README.md)
