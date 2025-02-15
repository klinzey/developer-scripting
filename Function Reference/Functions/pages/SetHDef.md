# SetHDef

## Description
Procedure SetHDef replaces the definition of the referenced &amp;quot;container&amp;quot; object with a new definition. Supported object types are worksheets, symbol definitions, and layer references.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetHDef(
				oldH : HANDLE;
				newH : HANDLE);
```

```python

def vs.SetHDef(oldH, newH):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|oldH|HANDLE|Handle to object.|
|newH|HANDLE|Handle to new definition.|

## Examples
```pascal
SetHDef(symbolHd,newSymDefHd);

{updates the referenced symbol with a new definition}
```

## Version
Availability: from MiniCAD6.0
## Category
* Object Editing

