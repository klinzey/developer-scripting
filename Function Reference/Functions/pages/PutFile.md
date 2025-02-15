# PutFile

## Description
Procedure PutFile displays a standard file dialog which requests the user to select or create a text file for output.&lt;BR&gt;


```pascal
PROCEDURE PutFile(
				commentStr   : DYNARRAY[] of CHAR;
				defaultStr   : DYNARRAY[] of CHAR;
				VAR fileName : DYNARRAY[] of CHAR);
```

```python

def vs.PutFile(commentStr, defaultStr):
    return fileName
```

## Parameters
|Name|Type|Description|
|---|---|---|
|commentStr|DYNARRAY[] of CHAR|User prompt string for dialog.|
|defaultStr|DYNARRAY[] of CHAR|Default file name string.|
|fileName|DYNARRAY[] of CHAR|Returns name of the user selected file.|

## Examples
```pascal
PROCEDURE PutFileExample;

VAR

	fileName :STRING;

BEGIN

	PutFile('Select the file to create:', 'New File.txt', fileName);

	Message(fileName);

	IF NOT DidCancel THEN BEGIN

		WriteLn('some text');

		Close(fileName);

	END;

END;

RUN(PutFileExample);
```

## See Also
VS Functions:
[GetLastFileErr](GetLastFileErr.md)| [Rewrite](Rewrite.md)| [GetFile](GetFile.md)| [Open](Open.md)| [Close](Close.md)

## Version
Availability: from MiniCAD
## Category
* File I/O

