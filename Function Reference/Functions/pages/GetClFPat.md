# GetClFPat

## Description
Returns the fill or hatch pattern of the specified class. &lt;BR&gt;
&lt;BR&gt;
A positive return value in a range of 0 to 71 is the index of the bitmap fill pattern of the class. A negative value is the negative of the fill pattern index (index * -1).&lt;BR&gt;
&lt;BR&gt;
Fill patterns and their associated constants can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#fptable&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetClFPat(className : STRING) : LONGINT;
```

```python

def vs.GetClFPat(className):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|className|STRING|Name of class.|

## Remarks
Returns the fill pattern of the class named className.

## Examples
```pascal
pbFillStyl:= GetClFPat('Grassy Cover');
```

## Version
Availability: from VectorWorks8.0
## Category
* Classes

