# DisableModules

## Description
Disables modules.  The modules parameter is a bitfield indicating which modules to disable.

```pascal
PROCEDURE DisableModules(modules : LONGINT);
```

```python

def vs.DisableModules(modules):
    return None
```

## Parameters
|Name|Type|Description|
|---|---|---|
|modules|LONGINT|This modules parameter is a LONGINT value which contains a bit for each possible product module.  If a module is enabled, then the corresponding bit is set to 1.  If that module is disabled, then its bit is 0.  The table below contains selectors that can be used to interpret the results of this function.  To determine if a module is enabled, do a bitwise &quot;and&quot; operation with the selector and the value returned by this function.  See the usage example below.

<I>Table - GetEnabledModules Selectors</I><P>
<CENTER>
<TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3>
  <TR BGCOLOR=#000000> 
	<TH WIDTH=133> <CENTER>
		<FONT COLOR=#FFFFFF> Module </FONT> </CENTER></TH>
	<TH WIDTH=48> <CENTER>
		<FONT COLOR=#FFFFFF> Selector </FONT> </CENTER></TH>
	<TH WIDTH=297> <CENTER>
		<FONT COLOR=#FFFFFF> Description </FONT> </CENTER></TH>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		Foundation  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		0  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC>&nbsp; <CENTER>
		Vectorworks general purpose CAD.  </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		RenderWorks  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		1  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC>&nbsp; <CENTER>
		Advanced rendering features, lighting, textures.  </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		Architect  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		2  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC> <CENTER>
		Architectural features including advanced window, door, wall framing, 
		HVAC. </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		Landmark  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		4  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC> <CENTER>
		Site modeling and landscape design module. </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		Spotlight  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		8  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC> <CENTER>
		Theater lighting, set, and scenic design features.  </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		Mechanical  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		16  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC> <CENTER>
		Mechanical engineering module for designers and fabricators. 
	  </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133 BGCOLOR=#CCCCCC> <CENTER>
		Pro  </CENTER></TD>
	<TD WIDTH=48 BGCOLOR=#CCCCFF> <CENTER>
		32  </CENTER></TD>
	<TD WIDTH=297 BGCOLOR=#CCCCCC> <CENTER>
		Foundation for European market. </CENTER></TD>
  </TR>
  <TR> 
	<TD WIDTH=133>&nbsp; </TD>
	<TD WIDTH=48>&nbsp; </TD>
	<TD WIDTH=297>&nbsp; </TD>
  </TR>
</TABLE>
</CENTER>|

## Version
Availability: from VectorWorks10.0
## Category
* Utility

