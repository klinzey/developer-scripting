# WriteMac

## Description
Outputs the specified data to an ASCII text file. The variable length parameter list specifies the data to be written to the file. &lt;BR&gt;
&lt;BR&gt;
Parameters may be any valid data type, and data types may be mixed in a single call to the procedure. WriteMac leaves the file pointer positioned at the end of the last data value written to the file; any data subsequently written to the file will be appended to the end of this value.&lt;BR&gt;
&lt;BR&gt;
See the VectorScript Language Guide for details on formatting values using WriteLn.

```pascal
PROCEDURE WriteMac(z : ANY);
```

```python

def vs.WriteMac(z):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|z|ANY||

## Examples
```pascal
WriteMac(Value1);
```

## Version
Availability: from VectorWorks9.0
## Category
* File I/O

