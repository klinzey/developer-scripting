# SetDashStyleN

## Description
Procedure SetDashStyleN creates a new linestyle in a Vectorworks document. Parameter name defines the name of the linestyle, parameter swt defines whether the linestyle will be scaled with thickness, and parameter numPairs specifies the number of length pairs defining the linestyle.&lt;BR&gt;
&lt;BR&gt;
The linestyle is defined by up to five black/white length pairs, which are specified in parameters b1,w1 through b5,w5. The minimum length of any given black or white parameter is 1 point, or 1/72 of an inch, and the line specification must be in pairs.

```pascal
PROCEDURE SetDashStyleN(
				name     : STRING;
				swt      : BOOLEAN;
				numPairs : INTEGER;
				pair1    : REAL;
				pair2    : REAL;
				pair3    : REAL;
				pair4    : REAL;
				pair5    : REAL);
```

```python

def vs.SetDashStyleN(name, swt, numPairs, pair1, pair2, pair3, pair4, pair5):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|name|STRING||
|swt|BOOLEAN||
|numPairs|INTEGER||
|pair1|REAL||
|pair2|REAL||
|pair3|REAL||
|pair4|REAL||
|pair5|REAL||

## Examples
```pascal
SetDashStyle('My Dash Style', True,0,1&quot;,1/4&quot;,1/4&quot;,1/4&quot;);
```

## Version
Availability: from Vectorworks 2010
## Category
* Document Attributes

