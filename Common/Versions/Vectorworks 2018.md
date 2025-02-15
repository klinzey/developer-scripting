## Version Information

Vectorworks 2018 is a Unicode application. Internally, Vectorworks uses UTF-16. To provide easier transition of Vector Scripts, the script engine uses [UTF-8 Encoding](https://en.wikipedia.org/wiki/UTF-8).

First, all sources files for Vector Script should be in UTF-8 text file encoding with or without BOM (Byte Order Mark). This is most notable if the copy-right symbol is used. These files must be converted to UTF-8 before using them in Vectorworks 2018.

This change only affects scripts using non-Latin(low ASCII) characters. As contrast Vectorworks 2017 will use one byte for such characters (representing ASCII symbol in the OS current code page) In the new version, such characters are represented by multiple bytes.

This means that the type STRING, which has a limit of 255 bytes, is not variable limit if used with non-Latin characters. If your string uses 4-byte symbols, then STRING would be (255/4 =) 63 characters limit.

This might be very limiting to certain users. So, we are recommending the use of 'DYNARRAY OF CHAR' instead. We have updated most of the VectorScript API to support this type along with the STRING.

The type **CHAR** should be avoided as it represents a byte in Vectorworks 2018 and a byte doesn't not equal a symbol in UTF-8. A symbol should be represented by STRING or DYNARRAY OF CHAR.

This means that appending the result of [Chr](../../Function%20Reference/Functions/pages/Chr.md) into a string might lead to bad string, as [Chr](../../Function%20Reference/Functions/pages/Chr.md) will allow values >= 127 to be appended to the string, thus creating a corrupted UTF-8 string.

A new function [UniChr](../../Function%20Reference/Functions/pages/UniChr.md) was added to allow working with numeric representation of symbols and it returns a STRING.

## New Features

* [Install Plugins into the Current Workspace](../Tasks/Install%20Plugins%20into%20the%20Current%20Workspace.md)
* [Binary File Operations](../Tasks/Binary%20File%20Operations.md)

## New Functions

[VS:Vectorworks 2018 New Functions](../VS:Vectorworks%202018%20New%20Functions.md)
