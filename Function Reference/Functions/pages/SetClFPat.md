# SetClFPat

## Description
Sets the fill pattern of the specified class.&lt;BR&gt;
&lt;BR&gt;
To apply a bitmap fill pattern, use a positive value corresponding to the desired fill pattern index. To apply a vector fill, use the negative of the index of the vector fill (index * -1).&lt;BR&gt;
&lt;BR&gt;
Fill patterns and their associated constants can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#fptable&quot;&gt;VectorScript Appendix&lt;/A&gt;.


```pascal
PROCEDURE SetClFPat(
				className   : STRING;
				fillpattern : LONGINT);
```

```python

def vs.SetClFPat(className, fillpattern):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|
|fillpattern|LONGINT|Fill pattern index value.|

## Remarks
Assigns a fill pattern to the class named className.

## Examples
```pascal
SetClFPat('Grassy Cover',42);
```

## Version
Availability: from VectorWorks8.0
## Category
* Classes

