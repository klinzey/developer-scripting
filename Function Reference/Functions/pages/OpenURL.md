# OpenURL

## Description
Opens a web page or file using the default browser or appropriate application (e.g. Adobe Acrobat).  Returns a boolean indicating the success of the operation.&lt;BR&gt;
&lt;BR&gt;
The URL (Uniform Resource Locator) is a pointer to a resource on the World Wide Web.  It specifies both the protocol and location of the document to open.  For files on the local computer, the URL should begin with file:// protocol specifier.  For web pages, the URL should begin with http://.  The URL should use forward slashes / to separate parts of the path.  &lt;BR&gt;
&lt;BR&gt;
There are some platform differences to be aware of.  Windows will accept either \ or / as the path separators.  MacOS X requires that file:// URLs begin with /Volumes/ before the drive name.  Also, currently the MacOS X implementation of OpenURL does not accept spaces in the URL.  Spaces should be replaced with the escape code %20 before calling this function.&lt;BR&gt;
&lt;BR&gt;
Note: The function GetFolderPath returns a string with separators specific for the platform it is running on (: on Mac and \ on Windows).  If your script calls this function to assemble a local file:// URL then you will have to replace the : separators with / characters. &lt;BR&gt;


```pascal
FUNCTION OpenURL(URLname : DYNARRAY[] of CHAR) : BOOLEAN;
```

```python

def vs.OpenURL(URLname):
    return BOOLEAN
```

## Parameters
|Name|Type|Description|
|---|---|---|
|URLname|DYNARRAY[] of CHAR|The Uniform Resource Locator for the web page or file to open. |

## Examples
```pascal
{ Open a webpage. }

	status := OpenURL('http://www.vectorworks.net');



	{ Open an HTML file on MacOS X. }

	status := OpenURL('file:///Volumes/MyMacXHD/Documents/My%20Files/Test.html');

	

	{ Open a PDF file in Acrobat on MacOS X. }

	status := OpenURL('file:///Volumes/MyMacXHD/Documents/My%20Files/VSLG11.pdf');



	{ Open a PDF file in Acrobat on MacOS 9. }

	status := OpenURL('file:///MyMac9HD/My Files/VSLG11.pdf');

	

	{ Open a PDF file in Acrobat on Windows. }

	status := OpenURL('file:///C:/My Files/VSLG11.pdf';

	


```

## Version
Availability: from VectorWorks10.0
## Category
* Utility

