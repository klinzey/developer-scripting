# BeginSym

## Description
Procedure BeginSym creates a new symbol definition ina Vectorworks document. &lt;BR&gt;
&lt;BR&gt;
Any objects created after a call to BeginSym will be included in the symbol definition. A call to EndSym will complete the creation of the symbol, which is then generated in the Vectorworks document.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE BeginSym(symbolName : STRING);
```

```python

def vs.BeginSym(symbolName):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|symbolName|STRING|Name of the new symbol.|

## Remarks
Note: normally SetOriginAbsolute(0,0) should be called before calling this. The user origin is used as the insertion point for the symbol, but it may be out of bounds, in which case the symbol is still created but the center of the document is used instead for the insertion point.

## Examples
```pascal
BeginSym('Window');

  Rect(-5'-11&quot;,-1&quot;,-2'-0&quot;,-5'-11&quot;);

  Rect(-5'-8 3/4&quot;,-2 1/4&quot;,-2'-2 1/4&quot;,-2'-10&quot;);

  Rect(-5'-8 3/4&quot;,-3'-1 3/4&quot;,-2'-2 1/4&quot;,-5'-9&quot;);

  Rect(-4'-7&quot;,-2'-7 3/4&quot;,-3'-3 1/2&quot;,-2'-9 1/2&quot;);

  MoveTo(-5'-11&quot;,-3'-0&quot;);

  LineTo(-2'-0&quot;,-3'-0&quot;);

EndSym;


```

## Version
Availability: from MiniCAD
## Category
* Objects - Symbols

