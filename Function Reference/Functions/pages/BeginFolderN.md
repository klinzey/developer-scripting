# BeginFolderN

## Description
Procedure BeginFolderN creates a new resource folder of the indicated type in a Vectorworks document. Any resource or folder of that type created after the current call to BeginFolderN will be nested inside the new folder. A call to EndFolder will complete the creation of the folder, which is then generated in the Vectorworks document.&lt;BR&gt;
&lt;BR&gt;
To name the new folder, precede BeginFolderN with a call to NameObject.&lt;BR&gt;


```pascal
PROCEDURE BeginFolderN(type : INTEGER);
```

```python

def vs.BeginFolderN(type):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|type|INTEGER|the type of resource the folder will contain|

## Examples
```pascal
const

kSymbolDefinitions = 16;

NameObject('Object Symbols');

BeginFolder(kSymbolDefinitions);

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
Availability: from Vectorworks 2018
## Category
* Document List Handling

