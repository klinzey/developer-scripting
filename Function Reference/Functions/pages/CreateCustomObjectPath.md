# CreateCustomObjectPath

## Description
Creates an instance of the path custom object specified by the name argument.  The vertices of the path are translated in such a way that the first vertex will be placed at the origin of the plug-in's coordinate space.

```pascal
FUNCTION CreateCustomObjectPath(
				objectName   : STRING;
				path         : HANDLE;
				profileGroup : HANDLE) : HANDLE;
```

```python

def vs.CreateCustomObjectPath(objectName, path, profileGroup):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|objectName|STRING|Name of object.|
|path|HANDLE|Handle to new object path polygon.|
|profileGroup|HANDLE|Handle to new profile group object.|

## Returns
Returns a HANDLE to the new path object.

## Remarks
Calls DefineCustomObject() first to either find the defining FormatNode or create it.  If it is created, the user will be presented with an initialization dialog.  Returns handle to Object.

## Examples
```pascal
PROCEDURE Example;

VAR

	h :HANDLE;

BEGIN

	CallTool(-204);

	h := CreateCustomObjectPath('Cutting Plane', FSActLayer, nil);

END;

RUN(Example);
```

## Version
Availability: from VectorWorks8.5
## Category
* Objects - Custom

