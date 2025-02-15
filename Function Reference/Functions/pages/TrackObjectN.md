# TrackObjectN

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
PROCEDURE TrackObjectN(
				traverseType : INTEGER;
				callback     : PROCEDURE;
				VAR outObj   : HANDLE;
				VAR p        : REAL);
```

```python

def vs.TrackObjectN(traverseType, callback):
    return (outObj, p)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|traverseType|INTEGER|Specify how to traverse the drawing.



0 - traverses only the high-level objects (the same as the TrakcObject function);



1 - traverses the objects deep (uses GetPickObjectInfo, the 'subH' parameter).



2 - traverses the objects shallow (uses GetPickObjectInfo|
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

	TrackObjectN( 0, CheckObjCallback, h, x, y, z );

	SetSelect( h );

END;

RUN( Test );


```

## See Also
VS Functions:
[TrackObject](TrackObject.md)| [GetPickObjectInfo](GetPickObjectInfo.md)

## Version
Availability: from Vectorworks 2014
## Category
* User Interactive

