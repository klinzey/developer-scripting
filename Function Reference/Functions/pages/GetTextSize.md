# GetTextSize

## Description
Procedure GetTextSize returns the text point size at a specified position within the referenced text object. 1 point = 1/72&amp;quot;. &lt;BR&gt;
&lt;BR&gt;
The position is in a range between 0 and 32767, representing a character position in the text string. An index of 0 refers to the first character in the string.

```pascal
FUNCTION GetTextSize(
				TextHd   : HANDLE;
				Position : INTEGER) : REAL;
```

```python

def vs.GetTextSize(TextHd, Position):
    return REAL
```

## Parameters
|Name|Type|Description|
|---|---|---|
|TextHd|HANDLE|Handle to text object.|
|Position|INTEGER|Position in text string.|

## Remarks
The result was previously an integer, but is now a floating point value. [9/14/98 - PCP]

## Version
Availability: from MiniCAD6.0
## Category
* Objects - Text

