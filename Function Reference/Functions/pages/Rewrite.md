# Rewrite

## Description
Procedure Rewrite creates a new ASCII text file or opens an existing one prior to writing data to the file.  If the file exists, new data written to the file will overwrite any data currently within the file.&lt;BR&gt;
&lt;BR&gt;
If the filename includes a fully qualified path, the path has to use the appropriate notation for the local operating system:&lt;br&gt; 
&lt;dir&gt;Macintosh HD:Applications:Vectorworks:Plug-Ins:Data:Notes.txt&lt;/dir&gt;
&lt;dir&gt;C:\Program Files\Vectorworks\Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename includes a path relative to the location of the Vectorworks executable, the subfolder delimiters have to be backslashes:&lt;br&gt;
&lt;dir&gt;Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename does not include a path, the file is assumed to exist in the same folder as the Vectorworks executable.

```pascal
PROCEDURE Rewrite(fileName : DYNARRAY[] of CHAR);
```

```python

def vs.Rewrite(fileName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Name of file.|

## Examples
```pascal
PROCEDURE Example;

VAR

   fileName :STRING; 

   major, minor, maintenance, platform :INTEGER;

BEGIN

   GetVersion(major, minor, maintenance, platform);

   IF platform = 1 THEN BEGIN

      fileName := '/Example.txt';

   END ELSE BEGIN

      fileName := 'C:\Example.txt';

   END;

   ReWrite(fileName);

   WriteLn('example text');

   Close(fileName);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* File I/O

