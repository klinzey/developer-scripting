# CreateLoftSurfaces

## Description
Creates NURBS surfaces by interpolating a group of cross-section curves.  The nurbs curves are lofted in the order in which they were added to the group.

```pascal
FUNCTION CreateLoftSurfaces(
				groupCurvesHd : HANDLE;
				bRule         : BOOLEAN;
				bClose        : BOOLEAN;
				bSolid        : BOOLEAN) : HANDLE;
```

```python

def vs.CreateLoftSurfaces(groupCurvesHd, bRule, bClose, bSolid):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|groupCurvesHd|HANDLE||
|bRule|BOOLEAN||
|bClose|BOOLEAN||
|bSolid|BOOLEAN||

## Examples
```pascal
PROCEDURE Example;

VAR

	h, groupHand :HANDLE;

	bRule, bClose, bSolid :BOOLEAN;

BEGIN

	BeginGroup;



	h := CreateNurbsCurve(-PLENGTH/2, 0, 0, true, 1);

	AddVertex3D(h, -PLENGTH/2,PHEIGHT,0);

	AddVertex3D(h, PLENGTH/2,PHEIGHT,0);

	AddVertex3D(h, PLENGTH/2,0,0);



	h := CreateNurbsCurve(-PLENGTH/2-POFFSET,0,pWidth, true, 1);

	AddVertex3D(h, -PLENGTH/2-POFFSET, PHEIGHT+POFFSET, pWidth);

	AddVertex3D(h, PLENGTH/2+POFFSET, PHEIGHT+POFFSET, pWidth);

	AddVertex3D(h, PLENGTH/2+POFFSET, 0, pWidth);



	EndGroup;

	groupHand := LNewObj;

	bRule := TRUE;

	bClose := FALSE;

	bSolid := FALSE;

	groupHand := CreateLoftSurfaces(groupHand, bRule, bClose, bSolid);

	SetRot3D(LNewObj,#90d,#0d,#0d,0,0,0);

END;

RUN(Example);


```

## Version
Availability: from VectorWorks10.0
## Category
* Objects - NURBS

