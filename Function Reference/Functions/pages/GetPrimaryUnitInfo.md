# GetPrimaryUnitInfo

## Description
Procedure GetPrimaryUnitInfo returns the primary units settings for the active document. &lt;BR&gt;


```pascal
PROCEDURE GetPrimaryUnitInfo(
				VAR style    : INTEGER;
				VAR prec     : LONGINT;
				VAR dimPrec  : LONGINT;
				VAR format   : INTEGER;
				VAR angPrec  : INTEGER;
				VAR showMark : BOOLEAN;
				VAR dispFrac : BOOLEAN);
```

```python

def vs.GetPrimaryUnitInfo():
    return (style, prec, dimPrec, format, angPrec, showMark, dispFrac)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|style|INTEGER|Returns active primary units style.|
|prec|LONGINT|Returns display precision.|
|dimPrec|LONGINT|Returns dimension precision.|
|format|INTEGER|Returns decimal formatting.|
|angPrec|INTEGER|Returns angular precision.|
|showMark|BOOLEAN|Returns unit mark display setting.|
|dispFrac|BOOLEAN|Returns fractional display setting.|

## Remarks
Returns settings information for primary units.

## Examples
```pascal
PROCEDURE Example;

VAR

	style              :INTEGER;

	prec, dimPrec      :LONGINT;

	format, angPrec    :INTEGER;

	showMark, dispFrac :BOOLEAN;

	major, minor, maintenance, platform :INTEGER;

BEGIN

	GetVersion(major, minor, maintenance, platform);

	GetPrimaryUnitInfo(style, prec, dimPrec, format, angPrec, showMark, dispFrac);



	CASE major of

		8: Case style of

			0: AlrtDialog('Custom');

			1: AlrtDialog('Old Style Feet/Inches');

			2: AlrtDialog('Millimeter');

			3: AlrtDialog('Centimeter');

			4: AlrtDialog('Inches');

			5: AlrtDialog('Meters');

			6: AlrtDialog('Feet/Inches');

			7: AlrtDialog('Feet');

		END;



		9..11: Case style of

			0: AlrtDialog('Custom');

			1: AlrtDialog('Feet/Inches');

			2: AlrtDialog('Feet');

			3: AlrtDialog('Inches');

			4: AlrtDialog('Millimeters');

			5: AlrtDialog('Centimeters');

			6: AlrtDialog('Meters');

		END;



		12: Case style of

			1: AlrtDialog('Feet and Inches');

			2: AlrtDialog('Inches');

			3: AlrtDialog('Feet');

			4: AlrtDialog('Yards');

			5: AlrtDialog('Miles');

			6: AlrtDialog('Microns');

			7: AlrtDialog('Millimeters');

			8: AlrtDialog('Centimeters');

			9: AlrtDialog('Meters');

			10: AlrtDialog('Kilometers');

			11: AlrtDialog('Degrees');

		END;



	END;

END; 

RUN(Example);
```

## See Also
VS Functions:
[GetRoundingBase](GetRoundingBase.md)

## Version
Availability: from VectorWorks8.0
## Category
* Units

