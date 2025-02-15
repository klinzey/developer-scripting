# CreateGradient

## Description
Creates a new gradient resource.

```pascal
FUNCTION CreateGradient(name : STRING) : HANDLE;
```

```python

def vs.CreateGradient(name):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING|A user-specified name by which the newly created gradient will be identified.|

## Returns
Returns a handle to a new gradient resource if successful, otherwise the function returns nil.

## Remarks
This function creates a default gradient with 2 color spots: a white color spot at position, 0.0, and a black color spot at position, 1.0.<BR>
A gradient resource must always have at least 2, but no more than 32767 color spots.<BR>
NOTE: if the specified name already exists, a unique nmae will be created by adding a number suffix to the specified name.<BR>


## Examples
```pascal
gradientHandle := CreateGradient('My Gradient');
```

## Version
Availability: from VectorWorks10.0
## Category
* Dialogs - Modern

