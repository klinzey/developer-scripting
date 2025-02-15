# GetOpacity

## Description
Gets the opacity of and object. Opacity is obtained as percentage value in range [0-100].

```pascal
PROCEDURE GetOpacity(
				h           : HANDLE;
				VAR opacity : INTEGER);
```

```python

def vs.GetOpacity(h):
    return opacity
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|The object which opacity will be get.|
|opacity|INTEGER|Output parameter. Return the object's opacity as percentage value in range [0-100].|

## Version
Availability: from VectorWorks 2008
## Category
* Object Attributes

