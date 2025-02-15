# ClipSurface

## Description
Creates a new surface object by subtracting the intersection of surfaces s1 and s2 from s1.&lt;BR&gt;


```pascal
PROCEDURE ClipSurface(
				s1 : HANDLE;
				s2 : HANDLE);
```

```python

def vs.ClipSurface(s1, s2):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|s1|HANDLE|Handle to object.|
|s2|HANDLE|Handle to object.|

## Examples
```pascal
PROCEDURE ClipSurfaceExample;

VAR

	h1, h2, h3 :HANDLE;

BEGIN

	DSelectAll;

	CallTool(-203);

	h1 := FSActLayer;

	DSelectAll;

	CallTool(-203);

	h2 := FSActLayer;

	ClipSurface(h1, h2);

	h3 := PrevObj(h2);

	IF h3 &lt;&gt; h1 THEN SetFPat(h3, 5);

END;

RUN(ClipSurfaceExample);


```

## Version
Availability: from VectorWorks8.5
## Category
* Objects - 2D

