# AutoKey

## Description
Function AutoKey returns TRUE if a non-modifier keyboard character has been continually depressed for longer than the system defined key repeat rate. If a keyboard character has been continually depressed, then ASCII code of the character is returned in parameter asciiCode.&lt;BR&gt;
&lt;BR&gt;
Modifier keys are defined as the Caps Lock, Command, Control, Option, and Shift keys.&lt;BR&gt;


```pascal
FUNCTION AutoKey(VAR asciiCode : LONGINT) : BOOLEAN;
```

```python

def vs.AutoKey():
    return (BOOLEAN, asciiCode)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|asciiCode|LONGINT|The ASCII code of the key depressed.|

## Examples
```pascal
WHILE NOT AutoKey(keyHit) DO

BEGIN

     SysBeep;

     SysBeep;

END;

Message('The key pressed was ',keyHit);


```

## Version
Availability: from MiniCAD
## Category
* User Interactive

