# SetFPat

## Description
Procedure SetFPat sets the fill pattern of the referenced object.&lt;BR&gt;
&lt;BR&gt;
To apply a bitmap fill pattern, use positive value corresponding to the index  of the bitmap pattern.  To apply a vector fill pattern, use the negative of the vector fill index (index * -1).&lt;BR&gt;
&lt;BR&gt;
Fill patterns and their associated constants can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#fptable&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;


```pascal
PROCEDURE SetFPat(
				h           : HANDLE;
				fillPattern : LONGINT);
```

```python

def vs.SetFPat(h, fillPattern):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|
|fillPattern|LONGINT|Fill index value.|

## Examples
```pascal
{ Apply a bitmap fill pattern. }

SetFPat(objectOne, 47);



{ Apply a vector fill. }

SetFPat(objectTwo, -Name2Index('My Hatch'));


```

## Version
Availability: from MiniCAD
## Category
* Object Attributes

