# Write

## Description
Procedure Write outputs the specified data to an ASCII text file. The variable length parameter list specifies the data to be written to the file. &lt;BR&gt;
&lt;BR&gt;
Parameters may be any valid data type, and data types may be mixed in a single call to the procedure. Write leaves the file pointer positioned at the end of the last data value written to the file; any data subsequently written to the file will be appended to the end of this value.&lt;BR&gt;
&lt;BR&gt;
See the VectorScript Language Guide for details on formatting values using WriteLn.

```pascal
PROCEDURE Write(z : ANY);
```

```python

def vs.Write(z):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|z|ANY||

## Examples
```pascal
Write(Value1);
```

## Version
Availability: from MiniCAD
## Category
* File I/O

