# ShowWSDialog

## Description
Displays a worksheet preference or settings dialog for the active worksheet. &lt;BR&gt;
&lt;BR&gt;
Settings or attributes modified by the dialog will be applied to the current selection range of the worksheet.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Worksheet Dialog Selectors&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH&gt;&lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt;Index&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH&gt;&lt;CENTER&gt;&lt;FONT COLOR=#FFFFFF&gt;Dialog&lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt;&lt;CENTER&gt;0&lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt;&lt;CENTER&gt;Column Width &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;1&lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;Cell Border&lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		2 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Number &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		3 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Preferences &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		4 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Print Setup &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD HEIGHT=17 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		5 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD HEIGHT=17 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Print &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		6 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Function &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		7 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Criteria &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		8 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Format Text &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		9 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Set Row Criteria &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		10 &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		Edit Row Criteria &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;

```pascal
PROCEDURE ShowWSDialog(dialogType : INTEGER);
```

```python

def vs.ShowWSDialog(dialogType):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|dialogType|INTEGER|Index of dialog to be displayed.|

## Remarks
Dialog Type constants:<BR>
Column Width		= 0<BR>
Cell Border		= 1<BR>
Number                        	= 2<BR>
Preferences		= 3<BR>
Print Setup		= 4<BR>
Print			= 5<BR>
Function			= 6<BR>
Criteria			= 7<BR>
Format Text		= 8<BR>
Set Row Criteria		= 9<BR>
Edit Row Criteria	                 = 10

## Version
Availability: from VectorWorks9.0
## Category
* Worksheets

