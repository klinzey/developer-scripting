# GetVWRString

## Description
Replaces GetResourceString -- load a string from VWR file

```pascal
PROCEDURE GetVWRString(
				VAR outputString : DYNARRAY[] of CHAR;
				resIdentifier    : DYNARRAY[] of CHAR;
				stringIdentifier : DYNARRAY[] of CHAR);
```

```python

def vs.GetVWRString(resIdentifier, stringIdentifier):
    return outputString
```

## Parameters
|Name|Type|Description|
|---|---|---|
|outputString|DYNARRAY[] of CHAR|result value|
|resIdentifier|DYNARRAY[] of CHAR|VWR identifier and path to vwstrings file|
|stringIdentifier|DYNARRAY[] of CHAR|key in vwstrings file|

## Version
Availability: from Vectorworks 2014
## Category
* Strings

