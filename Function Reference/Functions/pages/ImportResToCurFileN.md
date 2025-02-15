# ImportResToCurFileN

## Description
Imports the indicated resource from the specified list to the current file, if it is not already in the current file, and returns the handle to the resource. It will use a callback procedure to determine how to handle the duplicate resource. The function does a comparison between the resource being imported and the resources currently in the file. If there is an exact match, then is not not considered a conflict, the resource is not imported and the Callback procedure is not called.

```pascal
FUNCTION ImportResToCurFileN(
				listID   : LONGINT;
				index    : LONGINT;
				callback : PROCEDURE) : HANDLE;
```

```python

def vs.ImportResToCurFileN(listID, index, callback):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|listID|LONGINT||
|index|LONGINT||
|callback|PROCEDURE||

## Version
Availability: from Vectorworks 2014
## Category
* Document List Handling

