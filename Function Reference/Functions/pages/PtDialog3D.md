# PtDialog3D

## Description
Procedure PtDialog3D displays a dialog box which requests the user to enter a 3D coordinate (point) value.&lt;BR&gt;


```pascal
PROCEDURE PtDialog3D(
				displayStr : DYNARRAY[] of CHAR;
				xStr       : DYNARRAY[] of CHAR;
				yStr       : DYNARRAY[] of CHAR;
				zStr       : DYNARRAY[] of CHAR;
				VAR xPt    : REAL;
				VAR yPt    : REAL;
				VAR zPt    : REAL);
```

```python

def vs.PtDialog3D(displayStr, xStr, yStr, zStr):
    return (xPt, yPt, zPt)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|displayStr|DYNARRAY[] of CHAR|Dialog user prompt string.|
|xStr|DYNARRAY[] of CHAR|Default value for input field.|
|yStr|DYNARRAY[] of CHAR|Default value for input field.|
|zStr|DYNARRAY[] of CHAR|Default value for input field.|
|xPt|REAL|Returns user input X value.|
|yPt|REAL|Returns user input Y value.|
|zPt|REAL|Returns user input Z value.|

## Examples
```pascal
PtDialog3D('Enter the 3D location:','0','0','0',x,y,z);


```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined

