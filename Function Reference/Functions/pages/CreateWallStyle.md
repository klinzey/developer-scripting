# CreateWallStyle

## Description
Creates a new Wall Style of the give name.  If the name is already in use, the next available name will be used.

```pascal
FUNCTION CreateWallStyle(wallStyleName : STRING) : HANDLE;
```

```python

def vs.CreateWallStyle(wallStyleName):
    return HANDLE
```

## Parameters
|Name|Type|Description|
|---|---|---|
|wallStyleName|STRING|The name of the new Wall Style. If the name is already in use, the next available name will be used.|

## Returns
Returns a handle to the new Wall Style.

## Examples
```pascal
PROCEDURE Example;

CONST

   wallStyleName = 'Example Wall Style';

VAR

   wallStyleHandle :HANDLE;

   wdth :REAL;

   fill :LONGINT;

   pwLeft, pwRight, psLeft, psRight :INTEGER;

   boo :BOOLEAN;

BEGIN

   wallStyleHandle := CreateWallStyle(wallStyleName);

   wdth    := 1&quot;;

   fill    :=  1; {solid white}

   pwLeft  := 14; {in mils}

   pwRight := 14; {in mils}

   psLeft  :=  2; {solid black}

   psRight :=  2; {solid black}

   boo := InsertNewComponent(wallStyleHandle, 1, wdth, fill, pwLeft, pwRight, psLeft, psRight);

   SetName(wallStyleHandle, wallStyleName); {Reset the wall style name.}

END;

RUN(Example);


```

## Version
Availability: from VectorWorks12.5
## Category
* Objects - Walls

