## How to install

* Download the sample: ![PythonSample_ObjectPt2.zip](files/PythonSample_ObjectPt2.zip)
* Install the sample by copying the contents of the zip file into your user's 'Plug-ins' folder. The easiest way to find this folder is by going to Vectorworks menu Tools -> Options -> Vectorworks Preferences... then in the 'User Folder' tab click on 'Explore...' button and navigate to the 'Plug-ins' sub-folder.
**Note:** it is advisable to create a subfolder inside 'Plug-ins' and copy the sample files inside. This way all your plug-ins will be organized.
* Run Vectorworks and edit the Workspace (from the menu Tools -> Workspaces -> Workspace Editor) to add the new tool. It can be found under the 'Sample Python' category in the 'Tools' tab of the Workspace editor dialog.

## How the sample works

Similarly to the [Python Sample Menu Command](Python%20Sample%20Menu%20Command.md) sample, it uses an external py file to define the plug-in script and its parameters.

The script is a parametric object (see the parameters in the Plug-in Editor).

When the object in Vectorworks needs to be refreshed (e.g. when placed for the first time, when a parameter changes, etc.) the script code will be executed. The script will generate Vectorworks primitives ([LineTo](../../Function%20Reference/Functions/LineTo.md)) that will get added inside the object and those will form the visual appearance of the object.

In this sample, you can also see very primitive management of parameter visibility and enable/disable state.

## See Also

Python basic information: [Python](../README.md)

A simpler example can be found here: [Python Sample Menu Command](Python%20Sample%20Menu%20Command.md)

[Script Function Reference](../../Function%20Reference/README.md)
