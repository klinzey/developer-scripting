# GetCustomObjectColor

## Description
Get an auxilary color index stored in'objectHand' previously  with SetCustomObjectColor .  Aplication will preserve the color mapped to inTagID.

```pascal
FUNCTION GetCustomObjectColor(
				objectHand        : HANDLE;
				inTagID           : INTEGER;
				VAR outColorIndex : INTEGER) : BOOLEAN;
```

```python

def vs.GetCustomObjectColor(objectHand, inTagID):
    return (BOOLEAN, outColorIndex)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectHand|HANDLE|Handle to object.|
|inTagID|INTEGER||
|outColorIndex|INTEGER||

## Returns
Returns TRUE if the operation was successful.

## Examples
```pascal
PROCEDURE Example;

VAR

	objName :STRING;

	objHand, recHand, wallHand :HANDLE;

	colorIndexBefore, colorIndexAfter :INTEGER;

	boo :BOOLEAN;

BEGIN

	IF GetCustomObjectInfo(objName, objHand, recHand, wallHand) THEN BEGIN

		RGBToColorIndex(pRed, pGreen, pBlue, colorIndexBefore);

		Rect(0, 0, 1, 1);

		SetFillBack(LNewObj, colorIndexBefore);

		IF SetCustomObjectColor(objHand, 1, colorIndexBefore) THEN BEGIN

			boo := GetCustomObjectColor(objHand, 1, colorIndexAfter);

			AlrtDialog(Concat('before: ', colorIndexBefore, Chr(13), 'after: ', colorIndexAfter));

		END;

	END;

END;

RUN(Example);


```

## See Also
VS Functions:
[SetCustomObjectColor](SetCustomObjectColor.md)

## Version
Availability: from VectorWorks 2008
## Category
* Objects - Custom

