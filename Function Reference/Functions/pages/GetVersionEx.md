# GetVersionEx

## Description
Returns version information about the Vectorworks application. Parameter major returns the major version number of the application. Parameters minor and maintenance return minor version information. Parameter platform returns the OS platform on which Vectorworks is running (1 = Macintosh, 2 = Windows).&lt;BR&gt;
Parameter buildNum returns the build number of the version.&lt;BR&gt;
&lt;BR&gt;
Vectorworks 2008 has version major number 13, 2009 - 14 and so on.&lt;BR&gt;
&lt;BR&gt;
For example:&lt;BR&gt;
&lt;BR&gt;
Vectorworks 2010.0.1 running on a Macintosh would return:&lt;BR&gt;
&lt;BR&gt;
major: 15&lt;BR&gt;
minor: 0&lt;BR&gt;
maintenance: 1&lt;BR&gt;
platform: 1&lt;BR&gt;
buildNum: 95668&lt;BR&gt;


```pascal
PROCEDURE GetVersionEx(
				VAR major       : INTEGER;
				VAR minor       : INTEGER;
				VAR maintenance : INTEGER;
				VAR platform    : INTEGER;
				VAR buildNum    : LONGINT);
```

```python

def vs.GetVersionEx():
    return (major, minor, maintenance, platform, buildNum)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|major|INTEGER|Returns major version number of application.|
|minor|INTEGER|Returns minor version number of application.|
|maintenance|INTEGER|Returns maintenance version number of application.|
|platform|INTEGER|Returns platform of application.|
|buildNum|LONGINT|Returns the build number of application.|

## Examples
```pascal
PROCEDURE Example;

VAR 

	osMajor, osMinor, osIncr, buildNum :LONGINT; 

	appMajor, appMinor, appMaint, platform :INTEGER;

	platformStr :STRING;

BEGIN

	GetVersionEx(appMajor, appMinor, appMaint, platform, buildNum);

	GetOSVersion(osMajor, osMinor, osIncr);

	IF (platform = 1) 

		THEN platformStr := 'MacOS'

		ELSE platformStr := 'Windows';

	Message('Vectorworks ', appMajor, '.', appMinor, '.', appMaint, ' build ', buildNum, ' running on ', platformStr, ' ', osMajor, '.', osMinor, '.', osIncr);

END;

RUN(Example);


```

## Version
Availability: from Vectorworks 2010
## Category
* Utility

