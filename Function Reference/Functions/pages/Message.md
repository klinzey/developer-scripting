# Message

## Description
Procedure Message displays a floating message palette onscreen. Parameters z1 thru zN specify the values to be displayed in the palette. Parameters can be any supported data type or variables.&lt;BR&gt;
&lt;BR&gt;
If Message is called and the palette is already displayed, the value in the palette will be replaced by the new information. &lt;BR&gt;


```pascal
PROCEDURE Message(z : ANY);
```

```python

def vs.Message(z):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|z|ANY||

## Examples
```pascal
Message('Hello, world');



Message('The Number of objects was :',theNumber);

{displays a string using the variable value}
```

## Version
Availability: from MiniCAD
## Category
* Utility

