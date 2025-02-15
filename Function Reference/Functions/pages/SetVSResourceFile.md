# SetVSResourceFile

## Description
Sets the active resource file for a script. The resource file is opened for the duration of script execution.&lt;BR&gt;
&lt;BR&gt;
The name of the resource file should be specified without the file extension.

```pascal
FUNCTION SetVSResourceFile(fileName : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.SetVSResourceFile(fileName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|The name of the resource file to be opened.|

## Returns
A BOOLEAN value indicating the success of the file open operation.

## Remarks
Specify the file name without an extension. However, the file must exist in the plug-ins folder WITH an extension. Use .rsr on Windows and .rsrc on the Mac.

## See Also
VS Functions:
[GetResourceString](GetResourceString.md)

## Version
Availability: from VectorWorks9.0
## Category
* Dialogs - Modern

