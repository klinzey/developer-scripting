# GetObjectVariablePoint

## Description
Returns the value of a Vectorworks object property. Used with properties returning a 2D or 3D point value.&lt;BR&gt;
&lt;BR&gt;
For specific object selector index values, see the Appendix.

```pascal
FUNCTION GetObjectVariablePoint(
				h        : HANDLE;
				index    : INTEGER;
				VAR outP : REAL) : BOOLEAN;
```

```python

def vs.GetObjectVariablePoint(h, index):
    return (BOOLEAN, outP)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|index|INTEGER|Object property index.|
|outP|REAL|Return the object variable data point.|

## See Also
VS Functions:
[SetObjectVariablePoint](SetObjectVariablePoint.md)| [GetObjectVariableBoolean](GetObjectVariableBoolean.md)| [SetObjectVariableBoolean](SetObjectVariableBoolean.md)| [GetObjectVariableHandle](GetObjectVariableHandle.md)| [SetObjectVariableHandle](SetObjectVariableHandle.md)| [GetObjectVariableInt](GetObjectVariableInt.md)| [SetObjectVariableInt](SetObjectVariableInt.md)| [GetObjectVariableLongInt](GetObjectVariableLongInt.md)| [SetObjectVariableLongInt](SetObjectVariableLongInt.md)| [GetObjectVariableReal](GetObjectVariableReal.md)| [SetObjectVariableReal](SetObjectVariableReal.md)| [GetObjectVariableString](GetObjectVariableString.md)| [SetObjectVariableString](SetObjectVariableString.md)

## Version
Availability: from Vectorworks 2011
## Category
* Object Info

