# ReadLn

## Description
Procedure ReadLn will read data from a currently open text file. The variable length parameter list returns the read data in the specified parameters.&lt;BR&gt;
&lt;BR&gt;
Supported data types include INTEGER, REAL, LONGINT, CHAR or STRING. If the procedure encounters an EOF(end-of-file) marker, an error is generated. ReadLn positions the file position pointer to the beginning of a new line after the procedure is called.&lt;BR&gt;
&lt;BR&gt;
ReadLn will detect tabs as delimiters, allowing multiple string values to be assigned to variables.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE ReadLn(VAR z : ANY);
```

```python

def vs.ReadLn():
    return z
```

## Parameters
|Name|Type|Description|
|---|---|---|
|z|ANY||

## Examples
```pascal
PROCEDURE Example;

VAR

   fileName, value1, value2, value3 :STRING; 

   major, minor, maintenance, platform :INTEGER;

BEGIN

   GetVersion(major, minor, maintenance, platform);

   IF platform = 1 THEN BEGIN

      fileName := '/Example.txt';

   END ELSE BEGIN

      fileName := 'C:\Example.txt';

   END;

   Open(fileName);

   ReadLn(value1, value2, value3);

   Close(fileName);

   AlrtDialog(lineOfText);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* File I/O

