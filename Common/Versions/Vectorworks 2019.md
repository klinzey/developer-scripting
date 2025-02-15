## Version Information

### Unicode
Vectorworks 2019 is a Unicode application. Internally, Vectorworks uses UTF-16. To provide easier transition of Vector Scripts, the script engine uses [UTF-8 Encoding](https://en.wikipedia.org/wiki/UTF-8).

Similarly to Vectorworks 2018, all sources files for Vector Script should be in UTF-8 text file encoding with or without BOM (Byte Order Mark).

In contrast to previous versions, Vector Script STRING type size was increased from 255 to 2048 bytes, which translates to a different maximum number of characters, depending on the symbols used as in UTF-8 some symbols can be represented by 4 bytes (for example).

### Mac File Path Change
The Vectorscript functions [GetFile](../../Function%20Reference/Functions/pages/GetFile.md), [PutFile](../../Function%20Reference/Functions/pages/PutFile.md), [GetFolderPath](../../Function%20Reference/Functions/pages/GetFolderPath.md) and [FindFileInPluginFolder](../../Function%20Reference/Functions/pages/FindFileInPluginFolder.md) return a file path. For Vectorworks 2019, on the Macintosh platform, the path returned will be in the Posix format, rather than in the deprecated HFS format. If a Vectorscript calls one of these functions and passes the file path returned into another Vectorscript function, no change should be needed. If a Vectorscript calls one of these functions and checks that an HFS file path is returned on the Macintosh platform, the Vectorscript will probably need to be modified.

## New Features
- Line Type API Change, see [Line Type Reengineering Conversion Guide for Plug-ins](../Tasks/Line%20Type%20Reengineering%20Conversion%20Guide%20for%20Plug-ins.md)

## New Functions

[VS:Vectorworks 2019 New Functions](VS:Vectorworks 2019 New Functions)

## Obsoleted Functions

* [Obsolete Functions Table](Obsolete%20Functions%20Table.md)
