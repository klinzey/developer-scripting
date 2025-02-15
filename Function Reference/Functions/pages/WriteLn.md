# WriteLn

## Description
Procedure WriteLn outputs the specified data to an ASCII text file. The variable length parameter list specifies the data to be written to the file. &lt;BR&gt;
&lt;BR&gt;
Parameters may be any valid data type, and data types may be mixed in a single call to the procedure. A carriage return is appended to the end of the line of data, so that the file pointer is at the beginning of a new line in the file, and any data written to the file after the procedure call will be on the new line.&lt;BR&gt;
&lt;BR&gt;
See the VectorScript Language Guide for details on formatting values using WriteLn.&lt;BR&gt;


```pascal
PROCEDURE WriteLn(z : ANY);
```

```python

def vs.WriteLn(z):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|z|ANY||

## Examples
```pascal
PROCEDURE Example;

CONST

	Vendor = 'ACME';

	Price = 123.45;

	Tax = 1.07;

BEGIN

	ReWrite('Output.txt');

	WriteLn('Mfr/Cost: ', Vendor, '/', Price + Tax);

	Close('Output.txt');

END;

RUN(Example);


```

## See Also
VS Functions:
[WriteLnMac](WriteLnMac.md)

## Version
Availability: from MiniCAD
## Category
* File I/O

