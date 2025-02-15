# GetDrawingSizeRect

## Description
Returns  the top left and bottom right coordinates of a rectangle surrounding the entire area of the document containing objects.

```pascal
PROCEDURE GetDrawingSizeRect(
				VAR p1 : REAL;
				VAR p2 : REAL);
```

```python

def vs.GetDrawingSizeRect():
    return (p1, p2)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p1|REAL|Returns top left coordinate of drawing rectangle.|
|p2|REAL|Returns bottom right coordinate of drawing rectangle.|

## Remarks
Returns  the top left and bottom right coordinates of a rectangle surrounding the entire drawing.<BR>
<BR>
[sd 8/18/98]

## Version
Availability: from VectorWorks8.0
## Category
* Document Settings

