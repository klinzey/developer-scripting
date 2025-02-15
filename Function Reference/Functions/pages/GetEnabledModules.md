# GetEnabledModules

## Description
Determines which combination of product modules are currently enabled.  &lt;BR&gt;
&lt;BR&gt;
This function returns a LONGINT value which contains a bit for each possible product module.  If a module is enabled, then the corresponding bit will be set to 1.  If that module is disabled, then its bit will be 0.  The table below contains selectors that can be used to interpret the results of this function.  To determine if a module is enabled, do a bitwise &amp;quot;and&amp;quot; operation with the selector and the value returned by this function.  See the usage example below.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - GetEnabledModules Selectors&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR BGCOLOR=#000000&gt; 
	&lt;TH WIDTH=133&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Module &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH WIDTH=48&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Selector &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
	&lt;TH WIDTH=297&gt; &lt;CENTER&gt;
		&lt;FONT COLOR=#FFFFFF&gt; Description &lt;/FONT&gt; &lt;/CENTER&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Foundation  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		0  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;CENTER&gt;
		Vectorworks general purpose CAD.  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		RenderWorks  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		1  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt;&amp;nbsp; &lt;CENTER&gt;
		Advanced rendering features, lighting, textures.  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Architect  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		2  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Architectural features including advanced window, door, wall framing, 
		HVAC. &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Landmark  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		4  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Site modeling and landscape design module. &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Spotlight  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		8  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Theater lighting, set, and scenic design features.  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Mechanical  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		16  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Mechanical engineering module for designers and fabricators. 
	  &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Pro  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=48 BGCOLOR=#CCCCFF&gt; &lt;CENTER&gt;
		32  &lt;/CENTER&gt;&lt;/TD&gt;
	&lt;TD WIDTH=297 BGCOLOR=#CCCCCC&gt; &lt;CENTER&gt;
		Foundation for European market. &lt;/CENTER&gt;&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD WIDTH=133&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;TD WIDTH=48&gt;&amp;nbsp; &lt;/TD&gt;
	&lt;TD WIDTH=297&gt;&amp;nbsp; &lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;&lt;BR&gt;
&lt;BR&gt;


```pascal
FUNCTION GetEnabledModules : LONGINT;
```

```python

def vs.GetEnabledModules():
    return LONGINT
```

## Returns
A LONGINT bitfield value with a bit for each possible product module.

## Examples
```pascal
PROCEDURE testModules;



{----------------------------------------------------------}

FUNCTION bittest(value, mask :LONGINT) :BOOLEAN; 

VAR 

	bit :INTEGER; 

BEGIN 

	bittest := FALSE; 

	bit := 31;    { 2 ^ 31 is high order bit of a LONGINT argument. }

	WHILE ((bit &gt; -1) &amp; (bittest = false)) DO BEGIN 

		IF value &gt;= (2 ^ bit) THEN BEGIN 

			value := value - (2 ^ bit); 

			IF (2 ^ bit) = mask THEN bittest := TRUE; 

		END; 

		bit := bit - 1; 

	END; 

END; 





{----------------------------------------------------------}

FUNCTION IsModuleEnabled(whichModule :LONGINT) :BOOLEAN; 

VAR 

	enabledModules :LONGINT; 

BEGIN 

	enabledModules := GetEnabledModules; 

	IsModuleEnabled := bittest(enabledModules, whichModule)

END; 





BEGIN

	IF IsModuleEnabled(4) &amp; IsModuleEnabled(1)  THEN BEGIN

		{ Landmark and Renderworks are both enabled. } 

		{ ... }

	END;

END;

RUN(testModules);




```

## See Also
VS Functions:
[DisableModules](DisableModules.md)

## Version
Availability: from VectorWorks10.0
## Category
* Utility

