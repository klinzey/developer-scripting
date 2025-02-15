# KeyDown

## Description
Function KeyDown returns TRUE if a non-modifier keyboard character has been depressed. When TRUE is returned, the ASCII code of the character is returned.&lt;BR&gt;
&lt;BR&gt;
Modifier keys are the Caps Lock, Command, Control, Option, and Shift keys.&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION KeyDown(VAR asciiCode : LONGINT) : BOOLEAN;
```

```python

def vs.KeyDown():
    return (BOOLEAN, asciiCode)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|asciiCode|LONGINT|ASCII code of key pressed.|

## Examples
```pascal
WHILE NOT KeyDown(keyHit) DO

BEGIN

     SysBeep;

     SysBeep;

END;

Message('The key pressed was ',keyHit);

{an annoying example of one use of the KeyDown function}
```

## Version
Availability: from MiniCAD
## Category
* User Interactive

