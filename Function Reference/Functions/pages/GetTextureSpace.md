# GetTextureSpace

## Description
Function GetTextureSpace returns a handle to the texture space attached to the referenced object(or object part).

```pascal
FUNCTION GetTextureSpace(
				obj    : HANDLE;
				partID : INTEGER) : HANDLE;
```

```python

def vs.GetTextureSpace(obj, partID):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|partID|INTEGER|Part ID (pass 1 for non-supporting objects).|

## Remarks
Returns the texture space attached to this object, with the same part ID as partID.  Walls may have three texture spaces attached to them if they have expanded textures, for example.

## Examples
```pascal
PROCEDURE Example; 

VAR

	XAxis, YAxis, ZAxis :REAL; 

	hObj :HANDLE; 

BEGIN

	hObj := GetTextureSpace(FSActLayer, 0); 

	GetTexSpaceOrientU(hObj, XAxis, YAxis, ZAxis); 

	Writeln('U', ' : ', XAxis, ' : ', YAxis, ' : ', ZAxis); 

	GetTexSpaceOrientV(hObj, XAxis, YAxis, ZAxis); 

	Writeln('V', ' : ', XAxis, ' : ', YAxis, ' : ', ZAxis); 

	GetTexSpaceOrientW(hObj, XAxis, YAxis, ZAxis); 

	Writeln('W', ' : ', XAxis, ' : ', YAxis, ' : ', ZAxis); 

END; 

RUN(Example); 


```

## Version
```diff
- GetTextureSpace is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures

