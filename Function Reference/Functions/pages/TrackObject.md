# TrackObject

## Description
Interactively, including highlighting, allows the user to select one object meeting the specified criteria.&lt;BR&gt;
&lt;BR&gt;
The callback function (any of these depending on what info is needed):&lt;BR&gt;
&lt;BR&gt;
FUNCTION Callback(h : HANDLE): BOOLEAN;&lt;BR&gt;
FUNCTION CheckObjCallback(h : HANDLE; px, py : REAL) : BOOLEAN;&lt;BR&gt;
FUNCTION CheckObjCallback(h : HANDLE; px, py, pz : REAL) : BOOLEAN;&lt;BR&gt;
&lt;BR&gt;
is used to let the user filter the object that can be returned from the function.&lt;BR&gt;
&lt;BR&gt;
The parameteri px,py,pz pass into the function information about current cursor position in document units.&lt;BR&gt;
&lt;BR&gt;
This callback function is called when tracking over an object; also when click happens over an object.&lt;BR&gt;
&lt;BR&gt;
The callback function return true if the passed handle can be returned.

```pascal
PROCEDURE TrackObject(
				callback   : PROCEDURE;
				VAR outObj : HANDLE;
				VAR p      : REAL);
```

```python

def vs.TrackObject(callback):
    return (outObj, p)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|callback|PROCEDURE|The callback that will be called to check if an object meets the requrements to be tracked. See remarks.|
|outObj|HANDLE|Returns handle of the object for which the callback returned TRUE.|
|p|REAL|Returns coordinates of mouse click.|

## Examples
```pascal
PROCEDURE Test;

VAR

  h : HANDLE;

  x, y, z : REAL;

  

  FUNCTION CheckObjCallback(h : HANDLE) : BOOLEAN;

  {or FUNCTION CheckObjCallback(h : HANDLE; px, py : REAL) : BOOLEAN;}

  {or FUNCTION CheckObjCallback(h : HANDLE; px, py, pz : REAL) : BOOLEAN;}

  BEGIN

     {any object is ok}

     CheckObjCallback := true;

  END;



BEGIN

	TrackObject( CheckObjCallback, h, x, y, z );

	SetSelect( h );

END;

RUN( Test );


```

## Version
Availability: from Vectorworks 2010
## Category
* User Interactive

