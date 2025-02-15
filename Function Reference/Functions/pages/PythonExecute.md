# PythonExecute

## Description
Execute the given python script.&lt;BR&gt;
&lt;BR&gt;
You can use 'include' in python to run additional code in python files. However, before you execute the script make sure the python file are foundable through the PythonGetSearchPath. Use PythonSetSearchPath to change it.&lt;BR&gt;
&lt;BR&gt;
Scripts executed via this function should not contain User Interactive functions like GetPt for example.

```pascal
PROCEDURE PythonExecute(script : DYNARRAY[] of CHAR);
```

```python

def vs.PythonExecute(script):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|script|DYNARRAY[] of CHAR|The script to be executed.|

## See Also
VS Functions:
[PythonGetSearchPath](PythonGetSearchPath.md)| [PythonSetSearchPath](PythonSetSearchPath.md)

## Version
Availability: from Vectorworks 2014
## Category
* Utility

