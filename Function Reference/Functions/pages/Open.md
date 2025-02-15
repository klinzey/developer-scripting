# Open

## Description
Procedure Open opens a ASCII text file for reading.&lt;BR&gt;
&lt;BR&gt;
Remember to use Close when you are finished reading or writing to a file.&lt;BR&gt;
&lt;BR&gt;
If the filename includes a fully qualified path, the path has to use the appropriate notation for the local operating system:&lt;br&gt; 
&lt;dir&gt;Macintosh HD:Applications:Vectorworks:Plug-Ins:Data:Notes.txt&lt;/dir&gt;
&lt;dir&gt;C:\Program Files\Vectorworks\Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename includes a path relative to the location of the Vectorworks executable, the subfolder delimiters have to be backslashes:&lt;br&gt;
&lt;dir&gt;Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename does not include a path, the file is assumed to exist in the same folder as the Vectorworks executable.

```pascal
PROCEDURE Open(fileName : DYNARRAY[] of CHAR);
```

```python

def vs.Open(fileName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Name or path of file to open.|

## Examples
```pascal
PROCEDURE Example;

VAR

	fileName :STRING;

BEGIN

	UseDefaultFileErrorHandling(FALSE);

	fileName := 'Plug-Ins\Common\Data\Callout Prefs.txt';

	Open(fileName);

	AlrtDialog(Concat(GetLastFileErr));

	Close(fileName);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* File I/O

