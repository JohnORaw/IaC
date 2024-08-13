# Input and Output Redirection

In almost all command line environments, we have the concept of

1. A standard input device, normally the keyboard (STDIN=0)
2. A standard output device, normally the screen (STDOUT=1)
3. A standard error device, also normally the screen (STDERR=2)&#x20;

You may have seen these in the Linux shell, and we can also use them in Windows/DOS.&#x20;

At the command prompt, try typing **dir > rubbish.txt** and check what happened by typing **dir**. You should have a new file called rubbish.txt with whatever the output of the dir command was. You can check the contents with the command **more rubbish.txt** and you should do this. We have redirected the output of a command to a file using the operator **>**. This operator will create or overwrite the file. If we use the **>>** operator, it will append to the file.&#x20;

Now try the **help** command and look through the output. We need to become familiar with some of these commands, but we need to know how to identify all of them. Type **help > MyHelpFile.txt** and check to see that you have created a text file with a full listing of commands.
