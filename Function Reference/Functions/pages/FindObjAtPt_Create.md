# FindObjAtPt_Create

## Description
Creates object find for objects at specified point within specified radius. The funtion is capable of iterating

```pascal
FUNCTION FindObjAtPt_Create(
				hContainer  : HANDLE;
				objOptions  : INTEGER;
				travOptions : INTEGER;
				locX        : REAL;
				locY        : REAL;
				pickRadius  : REAL) : LONGINT;
```

```python

def vs.FindObjAtPt_Create(hContainer, objOptions, travOptions, locX, locY, pickRadius):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|hContainer|HANDLE||
|objOptions|INTEGER||
|travOptions|INTEGER||
|locX|REAL||
|locY|REAL||
|pickRadius|REAL||

## Version
Availability: from Vectorworks 2014
## Category
* Graphic Calculation

