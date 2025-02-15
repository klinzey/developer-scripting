# GetVPGroup

## Description
Gets the specified viewport group.&lt;BR&gt;
&lt;BR&gt;
groupType values:&lt;BR&gt;
Crop = 1&lt;BR&gt;
Annotation = 2&lt;BR&gt;
Cache = 3&lt;BR&gt;


```pascal
FUNCTION GetVPGroup(
				viewportHandle : HANDLE;
				groupType      : INTEGER) : HANDLE;
```

```python

def vs.GetVPGroup(viewportHandle, groupType):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|viewportHandle|HANDLE||
|groupType|INTEGER||

## Version
Availability: from VectorWorks11.0
## Category
* Objects - Groups

