# EOLN

## Description
Function EOLN returns TRUE if the file pointer of an open text file has reached a carriage return within the file. Parameter fileName specifies a text file which is open for reading or writing.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION EOLN(fileName : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.EOLN(fileName):
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

     WHILE NOT EOLN('MyData') DO

           Read(a,b,c,d);

      Close('MyData');

END;


```

## Version
Availability: from MiniCAD
## Category
* File I/O

