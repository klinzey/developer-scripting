# SetBBox

## Description
Procedure SetBBox positions objects whose geometry is defined by a bounding box. These objects currently are Image, PICT, Rectangle, Oval, Rounded Rectangle, and Worksheet Container. &lt;BR&gt;
&lt;BR&gt;
Other objects will generate a warning if they are passed to SetBBox.

```pascal
PROCEDURE SetBBox(
				h  : HANDLE;
				p1 : REAL;
				p2 : REAL);
```

```python

def vs.SetBBox(h, p1, p2):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|p1|REAL|Top left coordinate of bounding box.|
|p2|REAL|Bottom right coordinate of bounding box.|

## Remarks
This function should be obsleted and replaced by a function which can only move objects and not corrupt other bounding boxes. [PCP]<BR>
For objects which are defined by their box, such as rectangles &amp; ovals, this function allows that box to be changed.  [sd 8/14/98]

## Version
Availability: from MiniCAD
## Category
* Object Editing

