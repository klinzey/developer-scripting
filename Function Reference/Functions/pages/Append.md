# Append

## Description
Procedure Append opens the specified file for writing and appends the data to the end of the file. Existing data in the file is NOT overwritten.&lt;BR&gt;
&lt;BR&gt;
If the filename includes a fully qualified path, the path has to use the appropriate notation for the local operating system:&lt;br&gt; 
&lt;dir&gt;Macintosh HD:Applications:Vectorworks:Plug-Ins:Data:Notes.txt&lt;/dir&gt;
&lt;dir&gt;C:\Program Files\Vectorworks\Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename includes a path relative to the location of the Vectorworks executable, the subfolder delimiters have to be backslashes:&lt;br&gt;
&lt;dir&gt;Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename does not include a path, the file is assumed to exist in the same folder as the Vectorworks executable.

```pascal
PROCEDURE Append(fileName : DYNARRAY[] of CHAR);
```

```python

def vs.Append(fileName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Name of file to open for writing.|

## Examples
```pascal
PROCEDURE Example;

VAR

   fileName :STRING; 

   major, minor, maintenance, platform :INTEGER;

BEGIN

   GetVersion(major, minor, maintenance, platform);

   IF platform = 1 THEN BEGIN

      fileName := 'Macintosh HD:Example.txt';

   END ELSE BEGIN

      fileName := 'C:\Example.txt';

   END;

   Append(fileName);

   WriteLn('example text');

   Close(fileName);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* File I/O

