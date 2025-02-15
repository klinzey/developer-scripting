# SetObjExpandTexture

## Description
Procedure SetObjExpandTexture sets the &amp;quot;expanded&amp;quot; state of the referenced objects' texture. When a texture is expanded, different components of an object can have different textures.&lt;BR&gt;


```pascal
PROCEDURE SetObjExpandTexture(
				obj      : HANDLE;
				expanded : BOOLEAN);
```

```python

def vs.SetObjExpandTexture(obj, expanded):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj|HANDLE|Handle to object.|
|expanded|BOOLEAN|Use expanded textures setting.|

## Remarks
Sets whether three or just a single texture is applied to this object (can be up to three for walls or two for roofs).

## Version
```diff
- SetObjExpandTexture is obsolete as of Vectorworks 2009
```

Availability: from VectorWorks8.0
## Category
* Textures

