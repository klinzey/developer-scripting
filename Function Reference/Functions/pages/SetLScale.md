# SetLScale

## Description
Procedure SetLScale sets the scale of the referenced layer. &lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Calculating the Scale&lt;/I&gt;&lt;P&gt;
To calculate the scale parameter from an architecural scale, the following formula may be used :&lt;P&gt;

&lt;CENTER&gt;denominator/numerator * true size(in inches) = ActualSize&lt;/CENTER&gt;&lt;P&gt;

For example, to calculate a scale of 3/8&quot;=1'-0&quot;, the scale parameter would be 8/3 *12 = 32.


```pascal
PROCEDURE SetLScale(
				h     : HANDLE;
				scale : REAL);
```

```python

def vs.SetLScale(h, scale):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|h|HANDLE|Handle to layer.|
|scale|REAL|Scale value for layer.|

## Examples
```pascal
SetLScale(HandleToLayer,96);

{sets the referenced layer to a scale of 1/8&quot; = 1'}
```

## Version
Availability: from MiniCAD6.0
## Category
* Layers

