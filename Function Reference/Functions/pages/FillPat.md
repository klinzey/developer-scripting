# FillPat

## Description
Procedure FillPat sets the active fill pattern for the document. Any objects created after a calling this procedure will use the specified fill pattern.&lt;BR&gt;
&lt;BR&gt;
Fill patterns and their associated constants can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#fptable&quot;&gt;VectorScript Appendix&lt;/A&gt;.


```pascal
PROCEDURE FillPat(patNumber : LONGINT);
```

```python

def vs.FillPat(patNumber):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|patNumber|LONGINT|Index of fill pattern to be set as document default.|

## Examples
```pascal
Rect(0,0,2,2);

FillPat(21);

Rect(2,2,4,4);


```

## Version
Availability: from MiniCAD
## Category
* Document Attributes

