# RemoveGradientSliderSegment

## Description
Removes the specified segment from the gradient slider.&lt;BR&gt;
&lt;BR&gt;
Note: a gradient slider must always have at least 2 segments.

```pascal
PROCEDURE RemoveGradientSliderSegment(
				dialogID     : LONGINT;
				componentID  : LONGINT;
				segmentIndex : INTEGER);
```

```python

def vs.RemoveGradientSliderSegment(dialogID, componentID, segmentIndex):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogID|LONGINT|Index to the dialog layout that contains the gradient slider component.|
|componentID|LONGINT|Index to a specific gradient slider component.|
|segmentIndex|INTEGER|Index to segment to be removed.
(segment indexes begin with 1)|

## Examples
```pascal
RemoveGradientSliderSegment(dialogID, componentID, 4);
```

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern

