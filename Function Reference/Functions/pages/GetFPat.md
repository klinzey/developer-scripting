# GetFPat

## Description
Function GetFPat returns the fill pattern of the referenced object.&lt;BR&gt;
&lt;BR&gt;
A positive value corresponds to the index of the fill pattern on the pattern palette. A negative value corresponds to internal index of a vector fill pattern applied to the object.&lt;BR&gt;
&lt;BR&gt;
Fill patterns and their associated constants can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#fptable&quot;&gt;VectorScript Appendix&lt;/A&gt;.
&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetFPat(h : HANDLE) : LONGINT;
```

```python

def vs.GetFPat(h):
    return LONGINT
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to object.|

## Examples
```pascal
FPatValue:=GetFPat(HandleToObj);


```

## Version
Availability: from MiniCAD
## Category
* Object Attributes

