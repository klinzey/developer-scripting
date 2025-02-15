# SetClassN

## Description
Procedure SetClassN assigns a class to the referenced object.  &lt;BR&gt;
If the third parameter 'descIntoGroup' is set to true all objects within the group will receive the same class assignment as the group, &lt;BR&gt;
otherwise only the group itself will be affected.

```pascal
PROCEDURE SetClassN(
				h             : HANDLE;
				class         : STRING;
				descIntoGroup : BOOLEAN);
```

```python

def vs.SetClassN(h, class, descIntoGroup):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|class|STRING|Name of class to assign to object.|
|descIntoGroup|BOOLEAN|Assign the same class to all objects inside the group.|

## Examples
```pascal
{ select an object on drawing }

SetClassN(FSActLayer, 'Class Name-1', FALSE);
```

## See Also
VS Functions:
[SetClass](SetClass.md)

## Version
Availability: from Vectorworks 2018
## Category
* Object Attributes

