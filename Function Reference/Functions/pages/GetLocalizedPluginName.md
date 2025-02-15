# GetLocalizedPluginName

## Description
Get the localized name of a plug-in given its universal name.  &lt;BR&gt;
&lt;BR&gt;
When Vectorworks plug-ins are localized by distributors in other countries, their names are translated to the appropriate language.  The plug-in file stores both the original universal name and this translated localized name.  The translated name is displayed by the Vectorworks user interface instead of the original name.  If a script needs to display the name of a plug-in in a dialog or message then it should call this function to determine the localized name.  (Note that scripts will use the universal name to specify a plug-in when the name is not being displayed to the user.) &lt;BR&gt;
&lt;BR&gt;
If the plug-in has not been localized, then this function will return the universal name.

```pascal
FUNCTION GetLocalizedPluginName(
				inPluginName : STRING;
				VAR outName  : STRING) : BOOLEAN;
```

```python

def vs.GetLocalizedPluginName(inPluginName):
    return (BOOLEAN, outName)
```

## Parameters
|Name|Type|Description|
|---|---|---|
|inPluginName|STRING|Universal name of the plug-in.|
|outName|STRING|The localized name of the plug-in |

## Returns
Returns true if the specified plug-in exists, and false if it is not found.

## Examples
```pascal
PROCEDURE Example;

TYPE

	plugin = STRUCTURE

		universalName :STRING;

		localizedName :STRING;

		params :ARRAY[1..99,1..2] OF STRING;

		popups :ARRAY[1..99,1..99] OF STRING;

	END;

VAR

	plugins :ARRAY[1..99] OF plugin;

	cnt1, cnt2, cnt3, pluginCnt :INTEGER;

	str1, str2, str3, str4 :STRING;

	boo :BOOLEAN;

	int1, int2 :INTEGER;

	

PROCEDURE GetInfo(h :HANDLE);

VAR

	recHand :HANDLE;

	recName :STRING;

BEGIN

	recHand := GetRecord(h, NumRecords(h));

	recName := GetName(recHand);

	FOR cnt1 := 1 TO pluginCnt DO 

		IF recName = plugins[cnt1].universalName 

			THEN cnt1 := pluginCnt + 2;

	IF cnt1 &lt; pluginCnt + 2 THEN BEGIN

		boo := GetLocalizedPluginName(recName, str2);

		pluginCnt := pluginCnt + 1;

		plugins[pluginCnt].universalName := recName;

		plugins[pluginCnt].localizedName := str2;

		FOR cnt2 := 1 TO NumFields(recHand) DO BEGIN

			str1 := GetFldName(recHand, cnt2);

			int1 := GetFldType(recHand, cnt2);

			boo := GetLocalizedPluginParameter(recName, str1, str2);

			plugins[pluginCnt].params[cnt2, 1] := str1;

			plugins[pluginCnt].params[cnt2, 2] := str2;

			IF int1 = 8 THEN BEGIN

				FOR cnt3 := 1 TO NumCustomObjectChoices(recName, str1) DO BEGIN

					str3 := GetCustomObjectChoice(recName, str1, cnt3);

					boo := GetPluginChoiceIndex(recName, str1, str3, int2);

			  		boo := GetLocalizedPluginChoice(recName, str1, int2, str4);

			  		plugins[pluginCnt].popups[cnt2, cnt3] := Concat(str3, Chr(9), str4);

				END;

			END;

		END;

	END;

END;



BEGIN

	pluginCnt := 0;

	ForEachObject(GetInfo, (T=86));

	FOR cnt1 := 1 TO pluginCnt DO BEGIN

		WriteLn(plugins[cnt1].universalName, Chr(9), plugins[cnt1].localizedName);

		cnt2 := 1;

		WHILE plugins[cnt1].params[cnt2, 1] &lt;&gt; '' DO BEGIN

			WriteLn('    ', plugins[cnt1].params[cnt2, 1], Chr(9), plugins[cnt1].params[cnt2, 2]);

			cnt3 := 1;

			WHILE plugins[cnt1].popups[cnt2, cnt3] &lt;&gt; '' DO BEGIN

				WriteLn('        ', plugins[cnt1].popups[cnt2, cnt3]);

				cnt3 := cnt3 + 1;

			END;

			cnt2 := cnt2 + 1;

		END;

	END;

END;

RUN(Example);


```

## See Also
VS Functions:
[GetLocalizedPluginParameter](GetLocalizedPluginParameter.md)| [GetLocalizedPluginChoice](GetLocalizedPluginChoice.md)

## Version
Availability: from VectorWorks10.0
## Category
* Objects - Custom

