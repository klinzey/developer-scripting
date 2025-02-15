# GetDashLineTypeName

## Description
Retrieves the dash style name for the specified dash style using its negated internal index.

```pascal
FUNCTION GetDashLineTypeName(DashStyleIndex : LONGINT) : STRING;
```

```python

def vs.GetDashLineTypeName(DashStyleIndex):
    return STRING
```

## Parameters
|Name|Type|Description|
|---|---|---|
|DashStyleIndex|LONGINT|The negated internal index of the dash style.|

## Returns
Name of the dash style specified by the index.

## Remarks
This replaces GetDashStyleName

## See Also
VS Functions:
[SetDashLineTypeName](SetDashLineTypeName.md)

## Version
Availability: from Vectorworks 2019
## Category
* Object Names

