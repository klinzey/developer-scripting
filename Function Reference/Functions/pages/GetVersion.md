# GetVersion

## Description
Returns version information about the Vectorworks application. Parameter major returns the major version number of the application. Parameters minor and maintenance return minor version information. Parameter platform returns the OS platform on which Vectorworks is running (1 = Macintosh, 2 = Windows).&lt;BR&gt;
&lt;BR&gt;
Vectorworks 2008 has version major number 13, 2009 - 14 and so on.&lt;BR&gt;
&lt;BR&gt;
For example:&lt;BR&gt;
&lt;BR&gt;
Vectorworks 8.0.1 running on a Macintosh would return:&lt;BR&gt;
&lt;BR&gt;
major: 8&lt;BR&gt;
minor: 0&lt;BR&gt;
maintenance: 1&lt;BR&gt;
platform: 1&lt;BR&gt;


```pascal
PROCEDURE GetVersion(
				VAR major       : INTEGER;
				VAR minor       : INTEGER;
				VAR maintenance : INTEGER;
				VAR platform    : INTEGER);
```

```python

def vs.GetVersion():
    return (major, minor, maintenance, platform)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|major|INTEGER|Returns major version number of application.|
|minor|INTEGER|Returns minor version number of application.|
|maintenance|INTEGER|Returns maintenance version number of application.|
|platform|INTEGER|Returns platform of application.|

## Examples
```pascal
PROCEDURE Example;

VAR 

	osMajor, osMinor, osIncr :LONGINT; 

	appMajor, appMinor, appMaint, platform :INTEGER;

	platformStr :STRING;

BEGIN

	GetVersion(appMajor, appMinor, appMaint, platform);

	GetOSVersion(osMajor, osMinor, osIncr);

	IF (platform = 1) 

		THEN platformStr := 'MacOS'

		ELSE platformStr := 'Windows';

	Message('Vectorworks ', appMajor, '.', appMinor, '.', appMaint, ' running on ', platformStr, ' ', osMajor, '.', osMinor, '.', osIncr);

END;

RUN(Example);


```

## Version
Availability: from MiniCAD7.0
## Category
* Utility

