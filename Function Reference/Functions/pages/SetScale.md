# SetScale

## Description
Procedure SetScale sets the drawing scale of the active layer of the document.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Calculating the Scale&lt;/I&gt;&lt;P&gt;
To calculate the scale parameter from an architecural scale, the following formula may be used :&lt;P&gt;

&lt;CENTER&gt;denominator/numerator * true size(in inches) = ActualSize&lt;/CENTER&gt;&lt;P&gt;

For example, to calculate a scale of 3/8&quot;=1'-0&quot;, the scale parameter would be 8/3 *12 = 32.
&lt;BR&gt;
&lt;BR&gt;


```pascal
PROCEDURE SetScale(actualSize : REAL);
```

```python

def vs.SetScale(actualSize):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|actualSize|REAL|Drawing scale factor.|

## Version
Availability: from MiniCAD
## Category
* Layers

