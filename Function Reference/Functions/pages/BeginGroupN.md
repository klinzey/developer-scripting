# BeginGroupN

## Description
May be used to create objects in an existing group by passing a group handle; if a handle initialized to nil is passed a new group is created.

```pascal
PROCEDURE BeginGroupN(VAR groupHandle : HANDLE);
```

```python

def vs.BeginGroupN(groupHandle):
    return groupHandle
```

## Parameters
|Name|Type|Description|
|---|---|---|
|groupHandle|HANDLE|The group handle to be used; if handle is initialized to nil a new group is created.|

## Examples
```pascal
BeginGroupN(groupHandle);

  Rect(-1,1,0.5,0);

EndGroup;

{ adds created rect to existing group }



groupHandle := nil;

BeginGroupN(groupHandle);

  Rect(-1,1,0.5,0);

EndGroup;

{ creates new group and adds created rect to created group }
```

## See Also
VS Functions:
[BeginGroup](BeginGroup.md)| [EndGroup](EndGroup.md)

## Version
Availability: from Vectorworks 2011
## Category
* Objects - Groups

