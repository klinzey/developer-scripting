# AngDialog3D

## Description
Function AngDialog3D displays a dialog box which requests the user to enter three angle values. AngDialog3D will accept angle values in any supported angle format.&lt;BR&gt;


```pascal
PROCEDURE AngDialog3D(
				displayStr       : DYNARRAY[] of CHAR;
				xStr             : DYNARRAY[] of CHAR;
				yStr             : DYNARRAY[] of CHAR;
				zStr             : DYNARRAY[] of CHAR;
				VAR xAngleResult : REAL;
				VAR yAngleResult : REAL;
				VAR zAngleResult : REAL);
```

```python

def vs.AngDialog3D(displayStr, xStr, yStr, zStr):
    return (xAngleResult, yAngleResult, zAngleResult)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|displayStr|DYNARRAY[] of CHAR|Dialog user prompt string.|
|xStr|DYNARRAY[] of CHAR|Default value for input field.|
|yStr|DYNARRAY[] of CHAR|Default value for input field.|
|zStr|DYNARRAY[] of CHAR|Default value for input field.|
|xAngleResult|REAL|Returns user input X value.|
|yAngleResult|REAL|Returns user input Y value.|
|zAngleResult|REAL|Returns user input Z value.|

## Examples
```pascal
AngDialog3D('Enter the angle values:','0','0','0',x,y,z);
```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined

