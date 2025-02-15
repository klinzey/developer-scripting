# NoAngleVar

## Description
Sets the angle designation method in VectorScript. When called, VectorScript will treat language symbols which can be interpreted as direction angles (e.g., N, S, NW, SE) as as angles, rather than as variables.&lt;BR&gt;


```pascal
PROCEDURE NoAngleVar;
```

```python

def vs.NoAngleVar():
    return None
```

## Examples
```pascal
procedure test;

var

	S : Real;



begin

	NoAngleVar;

	S := 30;

	LineTo(3&quot;, #S);

	{ The 'S' will be treated as the direction 'South'  }

	{ and line will be drawn on 270 degree angle. }



end;

run(test);


```

## Version
Availability: from MiniCAD
## Category
* Command

