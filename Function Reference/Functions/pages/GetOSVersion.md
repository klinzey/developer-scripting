# GetOSVersion

## Description
Returns the version of the current operating system.

```pascal
PROCEDURE GetOSVersion(
				VAR major : LONGINT;
				VAR minor : LONGINT;
				VAR incr  : LONGINT);
```

```python

def vs.GetOSVersion():
    return (major, minor, incr)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|major|LONGINT|Major revision number|
|minor|LONGINT|Minor revision number|
|incr|LONGINT|Increment revision number|

## Examples
```pascal
PROCEDURE ShowVersionInfo;

VAR

	osMajor, osMinor, osIncr :LONGINT;

	vwMajor, vwMinor, vwMaint, platform: INTEGER;

	str :STRING;

BEGIN

	str := '';

	GetOSVersion(osMajor, osMinor, osIncr);

	GetVersion(vwMajor, vwMinor, vwMaint, platform);

	If platform = 1 then BEGIN

		str := Concat(str, 'Platform: Macintosh', chr(13));

		IF osMajor = 0 THEN osMajor := 10;

		str := Concat(str, 'OS Version: ', osMajor, '.', osMinor, '.', osIncr, chr(13));

	end else if platform = 2 then BEGIN

		str := Concat(str, 'Platform: Windows', chr(13));

		IF (osMajor = 4) &amp; (osMinor = 10) THEN str := Concat(str, 'OS Version: 98 SE', chr(13)) ELSE 

		IF (osMajor = 5) &amp; (osMinor =  1) THEN str := Concat(str, 'OS Version: XP',    chr(13)) ELSE 

		str := Concat(str, 'OS Version: ', osMajor, '.', osMinor, '.', osIncr, chr(13));

	END;

	str := Concat(str, 'VW Version: ', vwMajor, '.', vwMinor, '.', vwMaint);

	AlrtDialog(str);

END;

RUN(ShowVersionInfo);
```

## Version
Availability: from VectorWorks10.0
## Category
* Utility

