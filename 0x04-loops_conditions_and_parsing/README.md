The for loop is the first of the three shell looping constructs. This loop allows for specification of a list of values. A list of commands is executed for each value in the list.

The syntax for this loop is:

for NAME [in LIST ]; do COMMANDS; done

If [in LIST] is not present, it is replaced with in $@ and for executes the COMMANDS once for each positional parameter that is set (see Section 3.2.5 and Section 7.2.1.2).

The return status is the exit status of the last command that executes. If no commands are executed because LIST does not expand to any items, the return status is zero.

NAME can be any variable name, although i is used very often. LIST can be any list of words, strings or numbers, which can be literal or generated by any command. The COMMANDS to execute can also be any operating system commands, script, program or shell statement. The first time through the loop, NAME is set to the first item in LIST. The second time, its value is set to the second item in the list, and so on. The loop terminates when NAME has taken on each of the values from LIST and no items are left in LIST.

The while construct allows for repetitive execution of a list of commands, as long as the command controlling the while loop executes successfully (exit status of zero). The syntax is:

while CONTROL-COMMAND; do CONSEQUENT-COMMANDS; done

CONTROL-COMMAND can be any command(s) that can exit with a success or failure status. The CONSEQUENT-COMMANDS can be any program, script or shell construct.

As soon as the CONTROL-COMMAND fails, the loop exits. In a script, the command following the done statement is executed.

The return status is the exit status of the last CONSEQUENT-COMMANDS command, or zero if none was executed.
