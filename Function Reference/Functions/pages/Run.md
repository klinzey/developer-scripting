# Run

## Description
Initiates the execution of a VectorScript command by signalling the VectorScript interpreter to execute the script source code. &lt;BR&gt;
&lt;BR&gt;
The procedure takes a single parameter, which is the name of the VectorScript command as defined at the beginning of the source code listing.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE Run(p : PROCEDURE);
```

```python

def vs.Run(p):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|p|PROCEDURE||

## Examples
```pascal
PROCEDURE Example;

BEGIN

	Sysbeep;

	Sysbeep;

	Sysbeep;

END;

RUN(Example);


```

## Version
Availability: from MiniCAD
## Category
* Command

