# GetProjectUser

## Description
For a given userid in the current Project, get their full name and permission level.&lt;BR&gt;
&lt;BR&gt;
&lt;I&gt;Table - Project Sharing Permissions&lt;/I&gt;&lt;P&gt;
&lt;CENTER&gt;
&lt;TABLE BORDER=0 ALIGN=CENTER CELLSPACING=1 CELLPADDING=3&gt;
  &lt;TR&gt; 
	&lt;TH ALIGN=CENTER&gt;&lt;B&gt;Permission Level&gt;&lt;/B&gt;&lt;/TH&gt;
	&lt;TH ALIGN=CENTER&gt;&lt;B&gt;Constant&lt;/B&gt;&lt;/TH&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=LEFT&gt;Read Only&lt;/TD&gt;
	&lt;TD ALIGN=CENTER&gt;1&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=LEFT&gt;Layers-Restricted&lt;/TD&gt;
	&lt;TD ALIGN=CENTER&gt;2&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=LEFT&gt;Layers-Unrestricted&lt;/TD&gt;
	&lt;TD ALIGN=CENTER&gt;3&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=LEFT&gt;Layers and Resources&lt;/TD&gt;
	&lt;TD ALIGN=CENTER&gt;4&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=LEFT&gt;Project&lt;/TD&gt;
	&lt;TD ALIGN=CENTER&gt;5&lt;/TD&gt;
  &lt;/TR&gt;
  &lt;TR&gt; 
	&lt;TD ALIGN=LEFT&gt;Administrative&lt;/TD&gt;
	&lt;TD ALIGN=CENTER&gt;6&lt;/TD&gt;
  &lt;/TR&gt;
&lt;/TABLE&gt;
&lt;/CENTER&gt;


```pascal
FUNCTION GetProjectUser(
				userId         : STRING;
				VAR fullName   : STRING;
				VAR permission : INTEGER) : BOOLEAN;
```

```python

def vs.GetProjectUser(userId):
    return (BOOLEAN, fullName, permission)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|userId|STRING|The userid to look up|
|fullName|STRING|The users full name|
|permission|INTEGER|Permission level of the user|

## Returns
True on success, false on failure or not Project Sharing file.

## See Also
VS Functions:
[GetProjectUserNames](GetProjectUserNames.md)

## Version
Availability: from Vectorworks 2016
## Category
* Project Sharing

