# GetFile

## Description
Procedure GetFile displays a standard file dialog which requests the user to select a text document.&lt;BR&gt;
&lt;BR&gt;
It is advisable to call DidCancel after using this procedure and check that the user did not cancel the file selection process.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE GetFile(VAR fileName : DYNARRAY[] of CHAR);
```

```python

def vs.GetFile():
    return fileName
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Returns name of selected file.|

## Examples
```pascal
GetFile(fileName);

IF NOT DidCancel THEN BEGIN

     Read(a,b,c);

     Close(fileName);

END;

{Select a file for reading via a file open dialog}


```

## Version
Availability: from MiniCAD
## Category
* File I/O

