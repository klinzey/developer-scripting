# SetTool

## Description
Activates the specified Vectorworks tool for use. The tool remains selected as the active tool after use.&lt;BR&gt;
&lt;BR&gt;
Note: Please refer to the &lt;A HREF=&quot;../Appendix/appendix.html#settool&quot;&gt;VectorScript Appendix&lt;/A&gt; for specific tool ID values.
&lt;BR&gt;


```pascal
PROCEDURE SetTool(theTool : INTEGER);
```

```python

def vs.SetTool(theTool):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|theTool|INTEGER|Vectorworks tool constant.|

## Examples
```pascal
SetTool(-203);


```

## See Also
VS Functions:
[CallTool](CallTool.md)

## Version
Availability: from MiniCAD
## Category
* Command

