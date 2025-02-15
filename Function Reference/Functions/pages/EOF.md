# EOF

## Description
Function EOF returns TRUE if the file pointer of an open text file has reached the end of the file (EOF marker). Function EOF is used with Procedures Read and ReadLn to ensure proper file reading and closure. Parameter fileName specifies a text file which is open for reading or writing.&lt;BR&gt;
&lt;BR&gt;
If the filename includes a fully qualified path, the path has to use the appropriate notation for the local operating system:&lt;br&gt; 
&lt;dir&gt;Macintosh HD:Applications:Vectorworks:Plug-Ins:Data:Notes.txt&lt;/dir&gt;
&lt;dir&gt;C:\Program Files\Vectorworks\Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename includes a path relative to the location of the Vectorworks executable, the subfolder delimiters have to be backslashes:&lt;br&gt;
&lt;dir&gt;Plug-Ins\Data\Notes.txt&lt;/dir&gt;
If the filename does not include a path, the file is assumed to exist in the same folder as the Vectorworks executable.

```pascal
FUNCTION EOF(fileName : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.EOF(fileName):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|fileName|DYNARRAY[] of CHAR|Name of file.|

## Examples
```pascal
BEGIN

     Open('MyData');

     WHILE NOT EOF('MyData') DO

          ReadLn(a,b,c,d);

     Close('MyData');

END;


```

## Version
Availability: from MiniCAD
## Category
* File I/O

