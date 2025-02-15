## New Functions

[VS:Vectorworks 2011 New Functions](VS:Vectorworks 2011 New Functions)

## Deprecated Functions

**[GetType](../../Function%20Reference/Functions/pages/GetType.md)** -- deprecated due to 2D/3D Integration. This function will return -1 for 2D objects that are on a 3D plane. Use [GetTypeN](../../Function%20Reference/Functions/pages/GetTypeN.md) for the correct type.

**Note:** VW 2011 will rise warnings if the application preference "Stop Vectorscript on warnings" is TRUE when using:
* the deprecated routines from the previous version. The warning appears only once per session. Please check your code for the routines listed in [Obsolete Functions Table](Obsolete%20Functions%20Table.md).
* the Wall Style selectors from 1118 to 1157: use the new selectors instead starting 1177 (see SDK, MiniCadCallBacks.h)
