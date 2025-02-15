# BeginVectorFillN

## Description
Procedure BeginVectorFillN creates a new vector fill definition in a Vectorworks document. The value of vectorFillName will change only if the hatch name already exists.&lt;BR&gt;
&lt;BR&gt;
A color table listing with associated index values can be found in the &lt;A HREF=&quot;../Appendix/appendix.html#colors&quot;&gt;Appendix&lt;/A&gt;.


```pascal
PROCEDURE BeginVectorFillN(
				VAR vectorFillName : STRING;
				pageSpace          : BOOLEAN;
				rotateInWall       : BOOLEAN;
				colorIndex         : INTEGER);
```

```python

def vs.BeginVectorFillN(vectorFillName, pageSpace, rotateInWall, colorIndex):
    return vectorFillName
```

## Parameters
|Name|Type|Description|
|---|---|---|
|vectorFillName|STRING|Name of new vector fill pattern.|
|pageSpace|BOOLEAN|Sets page or world space for vector fill.|
|rotateInWall|BOOLEAN|Sets rotate in wall option for vector fill.|
|colorIndex|INTEGER|Background color of vector fill.|

## Remarks
Begins a hatch definition.  vectorFillName will return with a different name if the input name already is being used in the document.<BR>
<BR>
This is a new version of BeginVectorFill which returns the actual name of the hatch in the VAR STRING.

## Examples
```pascal
PROCEDURE CreateHatch;

VAR

	hatchName :STRING;

BEGIN

	hatchName := 'Default Hatch';

	BeginVectorFillN(hatchName, TRUE, FALSE, 0);

	AddVectorFillLayer(0,0,1,1,0.176776695,-0.176776695,1,1,255);

	EndVectorFill;

END;

RUN(CreateHatch);


```

## See Also
VS Functions:
[AddVectorFillLayer](AddVectorFillLayer.md)| [EndVectorFill](EndVectorFill.md)

## Version
Availability: from VectorWorks8.0
## Category
* Hatches / Vector Fills

