# GetMouse

## Description
Procedure GetMouse tracks and returns the current location of the cursor within the active Vectorworks document, allowing the cursor coordinates to be returned dynamically while moving the cursor onscreen.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE GetMouse(VAR p : REAL);
```

```python

def vs.GetMouse():
    return p
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|REAL|Returns current mouse coordinates.|

## Examples
```pascal
BEGIN

     WHILE NOT KeyDown(aCode) DO

     BEGIN

           GetMouse(CursX,CursY);

           Message('X : ',CursX,' Y : ',CursY);

     END;

END;

{displays the cursor coordinates as it is moved around onscreen}
```

## Version
Availability: from MiniCAD
## Category
* User Interactive

