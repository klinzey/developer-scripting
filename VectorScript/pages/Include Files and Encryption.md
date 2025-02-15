Include files used with scripts can be handled in one of two ways during the encryption process. Include files may be left
as unencrypted source code external to the script by appending a `.vss` extension to the file name. When the script
which references the include file is encrypted, the link to the file will be preserved, and the script will use the code
from the include file when executed. Scripts encrypted using this method still require the presence of the include file
in order to execute correctly.

> **Note:** Unencrypted include files which will be used with encrypted scripts should not reference subroutines, constants, or variables contained within the script. References to these items in an encrypted script will cause the script to fail.

Alternatively, include files can be encrypted along with the script which calls them by appending a `.px` extension to
the name of the include file. In this case, the contents of the include file are copied into the calling script and then the
entire body of source code is encrypted. The source code of the include file remains untouched by the encryption
process. Scripts encrypted in this manner do not require the presence of external include files to execute correctly, as
they contain all the needed code within the encrypted script.

For example, suppose the following procedure was in the include file `myinclude.vss` and was to be used in another
script:

```pascal
PROCEDURE Remote_Sub;
VAR
	j:INTEGER;
BEGIN
	AlrtDialog('This is the include function');
END;
```

The calling script then referenced the include file as shown:

```pascal
PROCEDURE EncryptExample1;
VAR
	i:INTEGER;
	s:STRING;
	
{$INCLUDE myinclude.vss}

BEGIN
	Remote_Sub;
END;
Run(EncryptExample1);
```

If the script above were encrypted, the subroutine `Remote_Sub` would remain in the include file. It would be called as
needed by the `EncryptExample1` script, and the include file would also need to be present in order for `EncryptExample1` to execute properly. If we were to change the name of the include file and modify the calling
script as shown:

```pascal
PROCEDURE EncryptExample1;
VAR
	i:INTEGER;
	s:STRING;

{$INCLUDE myinclude.px}

BEGIN
	Remote_Sub;
END;
Run(EncryptExample1);
```

In this instance, the code from `myinclude.px` would be copied into the calling script at the location of the include
statement, and the entire script would then be encrypted. The encrypted script would require no additional files to
execute properly, and the original code in the file `myinclude.px` would be untouched.

> **Note:** Include files should not be encrypted as standalone documents separate from a script. Files encrypted in such a manner cannot be referenced from another script, and cannot be decrypted.


## See Also
* [User Interface](User%20Interface.md)
* [Creating a Custom Dialog Box](Creating%20a%20Custom%20Dialog%20Box.md)
* [Plug-in Parameter Types](Plug-in%20Parameter%20Types.md)
* [Search Criteria](Search%20Criteria.md)
* [Include Files and Encryption](Include%20Files%20and%20Encryption.md)
* [Object Events](Object%20Events.md)
* [The VectorScript Debugger](The%20VectorScript%20Debugger.md)