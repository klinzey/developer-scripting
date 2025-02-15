# ConvertPosix2HSFPath

## Description
Machintosh only! &lt;BR&gt;
&lt;BR&gt;
Converts Posix (using '/' as delimiter) file path to HSF (using ':' as delimiter) file path.

```pascal
FUNCTION ConvertPosix2HSFPath(
				PosixPath      : DYNARRAY[] of CHAR;
				VAR outHSFPath : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.ConvertPosix2HSFPath(PosixPath):
    return (BOOLEAN, outHSFPath)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|PosixPath|DYNARRAY[] of CHAR|The Posix path that is to be converted.|
|outHSFPath|DYNARRAY[] of CHAR|Output parameter. Returns the converted path. If the function does not succeed the returned value is the passed 'PosixPath' value.|

## Returns
Returns true if the conversion succeeds. False if it fails.<BR>
The resulted Posix path will be the same as the passed Posix path if the function fails.

## See Also
VS Functions:
[ConvertHSF2PosixPath](ConvertHSF2PosixPath.md)

## Version
Availability: from Vectorworks 2010
## Category
* File I/O

