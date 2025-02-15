## What Scripts Can Do

Scripts provide the ability to perform most common programming tasks. Tasks such as computations, storing a value,
and manipulating data are all supported by standard constructs and methods within the language. Scripts also
provide extended capabilities specific to the Vectorworks product, adding new features not found in more generalized
languages.

### Object Creation and Editing

Scripts allow you to create and edit objects directly within a Vectorworks file. You can create primitive objects such as
lines as well as more complex objects such as multiple 3D extrudes or complex 3D solids. Scripts also provide the
ability to edit both the geometry and graphic attributes of these objects through extensive APIs built into the language.

### Document Control

Scripts provide APIs for controlling the various settings of individual Vectorworks files. These interfaces allow you to
retrieve and set geometric attributes of the file such as design layer scales or visibility, along with graphical attributes
such as fill or pen color.

### Extended Data

Scripts allow you to manipulate the extended data contained within the file to suit your specific needs. VectorScript
APIs provide access to and control over worksheets, data records, and textures which allow you to perform “deep
editing” of your files.

## What Scripts Can't Do

Your scripts can have an impressive range of capabilities; however, they are mostly confined to the scope of
Vectorworks and Vectorworks files. Since scripts are intended to be used within this context, they do not have features
that would be required for a standalone language:
* Scripts do not have the ability to work across multiple files or outside of a Vectorworks file context.
* For reasons of simplicity and stability, scripts do not have the ability to manage or control memory allocation.
* Scripts do not support system level calls for file‐related or other tasks.
* Scripts do not provide external database or other connectivity options.
* Finally, scripts do not provide multithreading capabilities.

## An Example Script

Letʹs take a look at a simple example to become more familiar with some of the basics of a typical script. The listing
below is an example of a small VectorScript which displays a message in the message bar, then clears the message after
five seconds:

```pascal
PROCEDURE FirstExample;
CONST
   kGREETING = 'Hello ';
VAR
   MyMessage : STRING;
BEGIN
   myMessage:='Script';

   Message(kGREETING,myMessage);
   Wait(5);
   SysBeep;
   ClrMessage;
END;
Run(FirstExample);
```

The program begins with a statement which names the procedure and identifies it to the VectorScript compiler:

```pascal
PROCEDURE FirstExample;   { Identifies the script to the VectorScript compiler }
CONST
	kGREETING = 'Hello ';
VAR
	myMessage : STRING;
BEGIN
	myMessage:='Script';
	
	Message(kGREETING,myMessage);
	Wait(5);
	SysBeep;
	ClrMessage;
END;
Run(FirstExample);
```

After this statement is what is known as the main program block. The main program block contains areas for declaring
what data storage will be needed by the script when it is run along with an area for the source code of the script, which
provides the instructions on what actions will be performed by the script:

```pascal
PROCEDURE FirstExample;
CONST
	kGREETING = 'Hello ';
VAR                           { Declares data storage for the script }
	myMessage : STRING;
	
BEGIN
	myMessage:='Script';
	Message(kGREETING,myMessage);
	Wait(5);
	SysBeep;              { The source code of the script }
	ClrMessage;
END;
Run(FirstExample);
```

The script ends with a special statement which tells the VectorScript compiler to execute the script code preceding it:

```pascal
PROCEDURE FirstExample;
CONST
	kGREETING = 'Hello ';
VAR
	myMessage : STRING;

BEGIN
	myMessage:='Script';

	Message(kGREETING,myMessage);
	Wait(5);
	SysBeep;
	ClrMessage;
END;
Run(FirstExample);     { Tells the VectorScript compiler to run the script }
```

Even though some of the concepts behind the parts of the script may not be clear to you at this point, studying the
example should give you an idea of what a script looks like and how it works. Later sections will explain the various
parts of a script and their underlying concepts in greater detail.

## Exploring Scripting

The best way to really learn any new programming language is to write programs with it. As you read through this
guide and through the [online function reference](../../Function%20Reference/README.md), you are encouraged to try out
features as you learn about them. There are several ways to do this, which make it easy to experiment with scripting
and learn about the languages.

The most basic way to explore scripts is to take a Vectorworks file and export it using the Export VectorScript
command. Once you have exported the file, open it in a text editor. What you will see is a VectorScript representation
of the complete Vectorworks file: objects, layers, classes, file settings, and so on. You can compare this script code to the
source file to see how a particular setting is created using VectorScript, or you can modify part of the script code and
import it into a blank file to see how your changes affect the file. You can also use parts of this script code in your own
scripts, either as‐is or as a basis for your own custom work.

Another useful technique for exploring scripts is to make use of the Custom Tool/Attribute and Custom Selection
commands of Vectorworks. These tool items make use of scripts to perform actions in Vectorworks, and you can use
them to explore how to use scripts. The Custom Tool/Attribute command lets you save graphical attribute and tool
settings for later use, and Custom Selection lets you define search criteria to select subsets of objects in your file. Both
these techniques can be very useful when writing your own scripts, and you can see how to use these techniques by
opening up the scripts and examining the script code.

Possibly the best technique is to start writing your own scripts from scratch. You can use the Resource Browser in
Vectorworks to create blank scripts and edit them through the Script Editor. The Script Editor provides several handy
features which give you quick access to API information and other basics of the language.

While exploring scripting, you will probably write scripts which don’t execute, or don’t work as you expected. To
correct problems which prevent your script from executing, you can check scriptʹs Error Output file, which will
indicate the source of any fatal errors in your scripts. To correct problems which are preventing your script from
working as desired, you can use the VectorScript debugger to trace through your code and locate the problem. You can
also use the basic technique used by many other languages—insert statements which display the values of relevant
variables in your script. VectorScript provides a convenient tool for this in the Message() statement.

Good luck with scripting, and have fun!


## See Also
* [User Interface](User%20Interface.md)
* [Creating a Custom Dialog Box](Creating%20a%20Custom%20Dialog%20Box.md)
* [Plug-in Parameter Types](Plug-in%20Parameter%20Types.md)
* [Search Criteria](Search%20Criteria.md)
* [Include Files and Encryption](Include%20Files%20and%20Encryption.md)
* [Object Events](Object%20Events.md)
* [The VectorScript Debugger](The%20VectorScript%20Debugger.md)