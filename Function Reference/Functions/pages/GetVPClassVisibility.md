# GetVPClassVisibility

## Description
Gets the visibility for the specified class in the specified viewport.

```pascal
FUNCTION GetVPClassVisibility(
				viewportHandle     : HANDLE;
				className          : STRING;
				VAR visibilityType : INTEGER) : BOOLEAN;
```

```python

def vs.GetVPClassVisibility(viewportHandle, className):
    return (BOOLEAN, visibilityType)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE||
|className|STRING||
|visibilityType|INTEGER||

## Version
Availability: from VectorWorks11.0
## Category
* Objects - Groups

