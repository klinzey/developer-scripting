# NameClass

## Description
Creates a new class in a Vectorworks document, which then become the active class.&lt;BR&gt;
If the specified class already exists, then it will become the active class of the document.&lt;BR&gt;
&lt;BR&gt;
Note: Class names cannot exceed 20 characters.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE NameClass(className : STRING);
```

```python

def vs.NameClass(className):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|

## Examples
```pascal
NameClass('Revisions');

Rect(4,4,6,6);



{Create a class 'Revisions' in the document}

{The rectangle is then assigned this class }


```

## Version
Availability: from MiniCAD
## Category
* Classes

