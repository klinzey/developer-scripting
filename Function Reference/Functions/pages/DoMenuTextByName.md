# DoMenuTextByName

## Description
Calls the specified Vectorworks menu command item.&lt;BR&gt;
&lt;BR&gt;
If the item is part of a Vectorworks menu chunk, pass the position of the item within the chunk as the second parameter. For menu items that are not part of a chunk, pass 0 as the second parameter.&lt;BR&gt;
&lt;BR&gt;
Note: DoMenuTextByName uses the internal Vectorworks menu item name to reference the menu command, and calls to this procedure will work on localized (international) versions of Vectorworks without modification. Note also that when calling VS plug-ins, you have to use the filename (which could be different from the internal plug-in name).&lt;BR&gt;
&lt;BR&gt;
A table listing DoMenuTextByName values can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#appx_h&quot;&gt;VectorScript Appendix&lt;/A&gt;.


```pascal
PROCEDURE DoMenuTextByName(
				subMenu : STRING;
				index   : INTEGER);
```

```python

def vs.DoMenuTextByName(subMenu, index):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|subMenu|STRING|Menu item  selector.|
|index|INTEGER|Menu chunk item position (range of 1 -  n).|

## Examples
```pascal
PROCEDURE DoMenuTextByNameExample;

BEGIN

	DoMenuTextByName('Print',0); {calls the print dialog}

	DoMenuTextByName('Standard Views',8); {sets view to right isometric}

END;

RUN(DoMenuTextByNameExample);


```

## Version
Availability: from MiniCAD5.0
## Category
* Command

