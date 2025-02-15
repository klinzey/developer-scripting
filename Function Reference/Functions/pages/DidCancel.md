# DidCancel

## Description
Function DidCancel detects whether the Cancel button in a predefined dialog was pressed. DidCancel is intended for use with conditional statements to signal that a cancel event has occurred.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION DidCancel : BOOLEAN;
```

```python

def vs.DidCancel():
    return BOOLEAN
```

## Examples
```pascal
PROCEDURE Example;

VAR

	i : INTEGER;

BEGIN

	i := IntDialog('Enter an integer:', '0');

	IF NOT DidCancel THEN BEGIN

		i := i*3;

		Message(i);

	END;

END;

RUN(Example);
```

## Version
Availability: from MiniCAD
## Category
* Dialogs - Predefined

