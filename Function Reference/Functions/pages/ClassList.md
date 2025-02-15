# ClassList

## Description
Returns the name of the specified class in the document class list. For example,  ClassList(4) will return the name of the fourth class in the list.

```pascal
FUNCTION ClassList(index : LONGINT) : STRING;
```

```python

def vs.ClassList(index):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|index|LONGINT|Index of class in class list (range of 1- n).|

## Remarks
NOTE: the manual has said that ClassLIst(4) returns the 4th class in the list, but it actually was returning the 5th class.  BF changed the function on 3/98 so it does return the 4th class.

## Examples
```pascal
noneClass := ClassList(1);

dimensionClass := ClassList(2);

classNumber3 := ClassList(3);

classNumber4 := ClassList(4);


```

## See Also
VS Functions:
[ClassNum](ClassNum.md)

## Version
Availability: from MiniCAD
## Category
* Classes

