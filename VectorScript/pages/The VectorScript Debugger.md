VectorScript provides a powerful tool to assist in solving problems that may occur while developing scripts. This tool,
known as a source‐level debugger, controls the execution so that the internal operations of the script can be observed
while the script is running. Using the debugger, it becomes possible to locate and solve problems by moving through
the script line by line to view the associated data, variables, and flow of script execution.

## Launching the Debugger

The VectorScript debugger is activated by using the `{$DEBUG}` compiler directive. This compiler directive, which can
be placed anywhere within a script, instructs the compiler to activate and display the debugger window when the
script is executed. For example,

```pascal
PROCEDURE MakeCircle;
{$DEBUG}
VAR
    x1,y1,x2,y2,radius : REAL;

BEGIN
    GetPt(x1,y1);
    GetPtL(x1,y1,x2,y2);
    radius:= Distance(x1,y1,x2,y2);
    Oval(x1 - radius,y1 + radius,x2 + radius,y2 - radius);
END;
Run(MakeCircle);
```

This launches the VectorScript debugger and displays the window as shown:

![Debugger Init](images/debuger_init.png)

The VectorScript debugger allows a script to be executed in a line‐by‐line fashion, also known as "stepping" through
the source code. The debugger performs this task beginning at the first line of the script and continuing through each
line until the end of the script is reached.

When the debugger is launched, storage for variables and constants is defined and script execution is paused at the
first line of code in the script body. The debugger window is then displayed, providing a wide array of information on
the script and the current state of execution.

## The Debugger Interface

![Debugger Window](images/debug_win.png)

The debugger window contains controls for managing script execution, as well as several areas for displaying various
data about the script and the state of execution.

### Debugger Controls

The debugger controls allow the execution of the script to be controlled during the debugging process. Script
execution can be started, stopped, paused, or advanced one line at a time.

![Debugger Controls](images/debug_controls.png)

The message area displays information about the script. These messages may include prompts for user interaction
with the script, script status information, or errors encountered in script execution.

See [Controlling Execution](#controlling-execution) for details on controlling script execution in the debugger.

### Script Calling Chain

The script calling chain pane displays the current function calling chain of the script. Each subroutine name appears
below the function calling it in the list; by highlighting the desired subroutine name, it is possible to determine which
subroutines are being called and the execution location within those subroutines.

### Script Source Code

The script source code pane displays the source code of the script being debugged. The current location of execution in
the script is indicated by the small blue arrow (![Blue Arrow](images/Blue_arrow.png)) on the left‐hand side of the pane. This arrow indicates the line of code that is about to be executed.

### Variable Data Display

The variable data display pane displays the current values stored in variables, arrays, and structures declared in the
script. The display is updated as execution proceeds, so that values can be continuously watched for changes during
execution.

Arrays, elements, and structure members may be displayed by clicking on the disclosure triangle (![Triangle](images/triangle.png)) that appears next to
the item.

## Controlling Execution

### Running a Script

To run the rest of the script without debugging, click the Run button.

![Run Button](images/debug_run.png)

### Continue the Execution of a Script

To continue the execution of the script until the script finishes or until the next break point, click the Continue Debug button.

![Continue Debug](images/contunue_debug.png)

Running scripts is primarily used in conjunction with setting a breakpoint in the debugger. For details on setting and
using breakpoints, see [Using Breakpoints](#using-breakpoints).

### Stepping Through a Single Line of a Script

To execute a single statement in the script, click the Step Over button.

![Step Over](images/step_over.png)

The Step Over button advances script execution by a single statement and refreshes the data display pane of the
debugger. The script position indicator advances to indicate the new location of script execution. If the statement
which is stepped through is a user defined subroutine, all the code within the subroutine is executed.

When stepping through a statement containing a user‐interactive function call (such as `GetPt()` or `GetLine()`), the
debugger dialog will be hidden and again will be shown after the function is executed.

### Stepping into a Subroutine

To advance execution into a user defined subroutine, click the Step Into button.

![Step Into](images/step_into.png)

The Step Into button is used when a statement containing a call to a user‐defined subroutine is reached. Whereas the
Step Over button will execute all the code contained within the subroutine and move to the next statement in the
calling function, Step Into will advance script execution to the first statement within the subroutine body.

The Step Into button performs a Step Over action with all other statements.

### Stepping Out of a Subroutine

To advance execution from the current script location in a subroutine to the next statement in the calling function, click
the Step Out button.

![Step Out](images/step_out.png)

When stepping out of a subroutine, all statements which follow the current script location will be executed, and script
execution will advance to the next statement in the calling routine.

### Stopping Script Execution

To terminate execution of a script, click the Terminate button.

![Terminate](images/stop_debug.png)

The Kill Script button will immediately terminate script execution. After the Kill Script button is pressed, the
debugger window will close.

## Using Breakpoints

A **breakpoint** suspends script execution and transfers control of the script to the debugger. When a breakpoint is
encountered, execution is suspended just prior to the breakpoint, and the script execution pointer is positioned at the
breakpoint location.

Breakpoints are often used in order to run scripts and stop them just prior to a statement or statements that are to be
debugged. Once the script has stopped at a breakpoint, it may be stepped through manually or by using the auto‐step
feature.

### Setting a Breakpoint

To set a breakpoint in the debugger, click the dash in the narrow column on the left side of the script source code pane.
The new break point will be indicated by a small diamond (![Breakpoint](images/breakpoint_white.png)) at the break location.

![Breakpoint Set](images/breakpoint.png)

Once a breakpoint has been set, the script can be executed using the Continue Debug button. Script execution will pause
when the breakpoint is reached, as indicated by a highlighted breakpoint and execution pointer arrow. The message
pane of the debugger will also indicate that a break point has been reached.

![Hit Breakpoint](images/hit_breakpoint.png)

To continue execution of the rest of the script **without debugging**, click the Run button. 

To continue execution using the VectorScript Debugger, click either the Continue Debug or Step Over/Into/Out buttons.

Breakpoints which have been placed in a looping statement will cause the script to stop each time the breakpoint is
encountered. When used in conjunction with the Continue Debug button, such breakpoints can be used to
observe conditions occurring within a loop during execution.

Care should be exercised when placing breakpoints within branching statements such as `IF..THEN` or `CASE`
statements. If the breakpoint is in a branch outside the path of execution, the script will continue to execute.

### Clearing Breakpoints

To clear a breakpoint in the debugger, click the diamond indicating the breakpoint location while script execution is
stopped or paused. The breakpoint is removed from the script.

## Viewing Data in the Debugger

Constant and variable data values may be observed during script execution in the data display pane of the debugger.
This pane displays all data storage locations declared in the script, as well as the values contained within them. The
data display pane is updated as each statement is executed, so changes in values can be observed as the script is
running.

![Variable Pane](images/variable_pane.png)

Vectors, array elements, and structure members can also be observed in the data display pane during script execution.
Items containing more than one storage location are shown with a disclosure triangle (![Triangle](images/triangle.png)) to the left of the item name. To
view the storage locations contained within the item, click the disclosure triangle; the individual locations and the
values contained in them will be displayed below the item name.

![Variable Data](images/debug_var2.png)

To edit the value of any variable data, click on the value. It would provide an extra dialog with an edit field to edit the corresponding value.

![Edit Value](images/edit_value.png)

To find faster and easier the variables in interest, a gray line will divide variables defined in different functions. The variables in each group will be sorted alphabetically.

![Variable Group](images/variable_03.png)



## See Also
* [User Interface](User%20Interface.md)
* [Creating a Custom Dialog Box](Creating%20a%20Custom%20Dialog%20Box.md)
* [Plug-in Parameter Types](Plug-in%20Parameter%20Types.md)
* [Search Criteria](Search%20Criteria.md)
* [Include Files and Encryption](Include%20Files%20and%20Encryption.md)
* [Object Events](Object%20Events.md)
* [The VectorScript Debugger](The%20VectorScript%20Debugger.md)
