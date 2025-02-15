# GetNumGradientSliderSegments

## Description
Gets the number of segments in the gradient slider.&lt;BR&gt;
&lt;BR&gt;
Note: a gradient slider must always have at least 2 segments.

```pascal
FUNCTION GetNumGradientSliderSegments(
				dialogID    : LONGINT;
				componentID : LONGINT) : INTEGER;
```

```python

def vs.GetNumGradientSliderSegments(dialogID, componentID):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the gradient slider component.|
|componentID|LONGINT|Index to a specific gradient slider component.|

## Returns
Retuns number of segments in gradient slider.<BR>
<BR>
(a segment consists of a color marker and the associated midpoint marker immediately to the right)

## Examples
```pascal
numSegments := GetNumGradientSliderSegments(dialogID, componentID);
```

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern

