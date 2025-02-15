# BeginText

## Description
Procedures BeginText creates a new text object in a Vectorworks document. All text specified between calls to BeginText and EndText will be part of the new text object.&lt;BR&gt;
Text may be specified in single quotes, or variables may be used..&lt;BR&gt;
&lt;BR&gt;
To specify the insertion point of the new text object, use TextOrigin.&lt;BR&gt;


```pascal
PROCEDURE BeginText;
```

```python

def vs.BeginText():
    return None
```

## Examples
```pascal
{ Create a multiple line text object at 0,0 }

TextFont(GetFontID('Monaco'));

TextSize(24);

TextOrigin(0,0);

BeginText;

'This multiple line text block 

is in 24pt Monaco and was created

by a VectorScript.'

EndText;


```

## Version
Availability: from MiniCAD
## Category
* Objects - Text

