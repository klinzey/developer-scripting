# StdReadLn

## Description
Procedure StdReadLn will read data from a currently open text file. The variable length parameter list returns the read data in the specified parameters.&lt;BR&gt;
&lt;BR&gt;
Supported data types include INTEGER, REAL, LONGINT, CHAR or STRING. Non STRING data values must be separated by a tab or space to be correctly read into variables. If the procedure encounters an EOF(end-of-file) marker, an error is generated. StdReadLn positions the file position pointer to the beginning of a new line after the procedure is called.&lt;BR&gt;
&lt;BR&gt;
StdReadLn reads data according to the Pascal language standard. This differs from the ReadLn procedure found in VectorScript primarily when reading STRING data. StdReadLn will read all characters, including tabs and spaces, as a single string value. ReadLn will detect tabs as delimiters, allowing multiple string values to be assigned to variables.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE StdReadLn(VAR z : ANY);
```

```python

def vs.StdReadLn():
    return z
```

## Parameters
|Name|Type|Description|
|---|---|---|
|z|ANY||

## Examples
```pascal
GetFile(fName);

IF NOT DidCancel THEN BEGIN

Open(fName);

StdReadLn(partID,partName);

END;
```

## Version
Availability: from VectorWorks8.0
## Category
* File I/O

