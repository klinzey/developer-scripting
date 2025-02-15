# CallTool

## Description
Activates the specified Vectorworks tool for a single use. After the tool has been used Vectorworks will revert back to the previously active tool.&lt;BR&gt;
&lt;BR&gt;
Note: Please refer to the &lt;A HREF=&quot;../Appendix/appendix.html#settool&quot;&gt;VectorScript Appendix&lt;/A&gt; for specific tool ID values.


```pascal
PROCEDURE CallTool(toolID : INTEGER);
```

```python

def vs.CallTool(toolID):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|toolID|INTEGER|Vectorworks tool constant.|

## Remarks
Changes the active tool to that specified by toolID. Waits until the user has executed the functionality of that tool, then switches back to the previously active tool &amp; returns.<BR>
<BR>
[sd 8/13/98]

## Examples
```pascal
PushAttrs;

PenFore(16);

PenBack(0);

PenPat(-2);

CallTool(-201);

PopAttrs;


```

## Version
Availability: from MiniCAD4.0
## Category
* User Interactive

