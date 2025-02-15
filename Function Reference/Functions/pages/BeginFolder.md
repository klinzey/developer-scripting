# BeginFolder

## Description
Procedure BeginFolder creates a new symbol folder in a Vectorworks document. Any symbols or symbol folders created after the current call to BeginFolder will be nested inside the new symbol folder. A call to EndFolder will complete the creation of the symbol folder, which is then generated in the Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
To name the new symbol folder, precede BeginFolder with a call to NameObject.&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE BeginFolder;
```

```python

def vs.BeginFolder():
    return None
```

## Examples
```pascal
NameObject('Object Symbols');

BeginFolder;

  BeginSym('Oval Symbols');

    PenSize(14);

    PenPat(2);

    FillPat(1);

    FillFore(0,0,0);

    FillBack(65535,65535,65535);

    PenFore(0,0,0);

    PenBack(65535,65535,65535);

    Oval(-1/4&quot;,1/4&quot;,3/4&quot;,-3/4&quot;);

  EndSym;

EndFolder;

{creates the symbol folder 'Object Symbols', which contains a symbol}
```

## Version
Availability: from MiniCAD
## Category
* Document List Handling

