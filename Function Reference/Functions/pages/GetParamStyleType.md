# GetParamStyleType

## Description
Returns the style type (by instance or by style) for a parameter.

```pascal
FUNCTION GetParamStyleType(
				hStyle    : HANDLE;
				paramName : STRING) : INTEGER;
```

```python

def vs.GetParamStyleType(hStyle, paramName):
    return INTEGER
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hStyle|HANDLE|Handle to a symbol containing a plug-in style.|
|paramName|STRING|Universal name of a parameter to check for style type.|

## Returns
0 = Parametrer is an instance parameter<BR>
1 = Parameter is a style parameter.<BR>
<BR>
If the object in unstyled or the parameter name if not found 0 will be returned and should be treated as an instance parameter.

## Version
Availability: from Vectorworks 2017
## Category
* Objects - Custom

