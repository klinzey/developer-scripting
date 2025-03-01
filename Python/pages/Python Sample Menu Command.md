## How to install

* Download the sample: ![PythonSample_Menu2.zip](files/PythonSample_Menu2.zip)
* Install the sample by copying the contents of the zip file into your user's 'Plug-ins' folder. The easiest way to find this folder is by going to Vectorworks menu Tools -> Options -> Vectorworks Preferences... then in the 'User Folder' tab click on 'Explore...' button and navigate to the 'Plug-ins' sub-folder.
**Note:** it is advisable to create a sub-folder inside 'Plug-ins' and copy the sample files inside. This way all your plug-ins will be organized.
* Run Vectorworks and edit the Workspace (from the menu Tools -> Workspaces -> Workspace Editor) to add the new menu command. It can be found under the 'Sample Python' category.

## How the sample works

The sample adds a new menu command defined by the 'vsm' file which represents a plug-in. You can see this plug-in under the menu Tools -> Plug-ins -> Plug-in Manager. There you can edit properties of the script as well as the script text itself.

The script for this sample 'import's python module (represented by a separate file) called '_main.py'. This module defines the behavior of the plug-in. 

```py
import _main
_main.execute()
```

When the sample menu command is executed, the script imports the '_main' module and runs the 'execute' function inside. It demonstrates how to show a dialog, collect some data, and act on the data.

## See Also

Python basic information: [Python](../README.md)

[Script Function Reference](../../Function%20Reference/README.md)
