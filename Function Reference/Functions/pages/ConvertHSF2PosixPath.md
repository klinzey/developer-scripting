# ConvertHSF2PosixPath

## Description
Machintosh only!&lt;BR&gt;
&lt;BR&gt;
Converts HSF (using ':' as delimiter) file path to Posix (using '/' as delimiter) file path.

```pascal
FUNCTION ConvertHSF2PosixPath(
				HSFPath          : DYNARRAY[] of CHAR;
				VAR outPosixPath : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.ConvertHSF2PosixPath(HSFPath):
    return (BOOLEAN, outPosixPath)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|HSFPath|DYNARRAY[] of CHAR|The HSF path that is to be converted.|
|outPosixPath|DYNARRAY[] of CHAR|Output parameter. Returns the converted path. If the function does not succeed the returned value is the passed 'HSFPath' value.|

## Returns
Returns true if the conversion succeeds. False if it fails.<BR>
The resulted Posix path will be the same as the passed HSF path if the function fails.

## See Also
VS Functions:
[ConvertPosix2HSFPath](ConvertPosix2HSFPath.md)

## Version
Availability: from Vectorworks 2010
## Category
* File I/O

