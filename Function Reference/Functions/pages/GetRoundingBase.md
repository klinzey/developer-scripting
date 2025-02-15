# GetRoundingBase

## Description
Gets the rounding base (1, 2.5, or 5) for the display, primary units, and secondary units.

```pascal
PROCEDURE GetRoundingBase(
				VAR display   : INTEGER;
				VAR primary   : INTEGER;
				VAR secondary : INTEGER);
```

```python

def vs.GetRoundingBase():
    return (display, primary, secondary)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|display|INTEGER|Rounding base for the display units|
|primary|INTEGER|Rounding base for the primary units|
|secondary|INTEGER|Rounding base for the secondary units|

## Examples
```pascal
FUNCTION DisplayAccuracy :REAL;

VAR

	dec_prec  :REAL;

	frac_prec :REAL;

	display   :INTEGER; 

	primary   :INTEGER; 

	secondary :INTEGER;

BEGIN

	GetRoundingBase(display, primary, secondary);

	dec_prec := 1 / (10 ^ GetPrefLongInt(169));

	IF display = 1 THEN dec_prec := dec_prec * 2.5 ELSE

	IF display = 2 THEN dec_prec := dec_prec * 5;

	frac_prec := 1 / (2 ^ GetPrefLongInt(171));

	IF NOT  GetPref(168) THEN DisplayAccuracy := dec_prec

	ELSE IF GetPref(175) THEN DisplayAccuracy := Min(dec_prec, frac_prec)

	ELSE DisplayAccuracy := frac_prec;

END;


```

## Version
Availability: from VectorWorks10.0
## Category
* Units

