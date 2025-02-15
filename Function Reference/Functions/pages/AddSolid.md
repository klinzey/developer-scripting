# AddSolid

## Description
Function AddSolid creates a new solid addition object from the referenced source objects. If the operation succeeds, the source objects will then be contained within the newSolid object, as the primitives which define the CSG.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Solids Operation Result Codes&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Operation Result&lt;/FONT&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER BGCOLOR=#000000&gt;&lt;FONT COLOR=#FFFFFF&gt;Result Code&lt;/FONT&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Success&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;0&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Null geometry error&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Geometry error&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Out of memory error&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Bad group error&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Invalid object type&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCCC&gt;Bad input&lt;/TD&gt;
	&lt;TD ALIGN=CENTER BGCOLOR=#CCCCFF&gt;20&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;


```pascal
FUNCTION AddSolid(
				obj1         : HANDLE;
				obj2         : HANDLE;
				VAR newSolid : HANDLE) : INTEGER;
```

```python

def vs.AddSolid(obj1, obj2):
    return (INTEGER, newSolid)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|obj1|HANDLE|Handle to source object for add operation.|
|obj2|HANDLE|Handle to source object for add operation.|
|newSolid|HANDLE|Handle to resultant object from add operation.|

## Examples
```pascal
PROCEDURE Example;

VAR

   h1, h2, h3 :HANDLE;

   int :INTEGER;

BEGIN

   DSelectAll; BeginXtrd(0, 1); CallTool(-203); h1 := FSActLayer; EndXtrd;

   DSelectAll; BeginXtrd(0, 1); CallTool(-203); h2 := FSActLayer; EndXtrd;

   int := AddSolid(h1, h2, h3);

END;

RUN(Example);
```

## Version
Availability: from MiniCAD7.0
## Category
* Objects - Solids

