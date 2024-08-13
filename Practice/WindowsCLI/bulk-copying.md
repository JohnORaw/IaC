# Bulk Copying

Some of the most common commands we use are those that allow us to copy. In DOS/Windows, try running the commands&#x20;

**help copy**&#x20;

**help xcopy**&#x20;

**help robocopy**&#x20;

We know how to use **copy **_**source destination**_ and the other commands are just a sophisticated version allowing recursive copies of files and directories to be copied.&#x20;

Go to your home directory and try the command **xcopy .\CLI .\CLI2**&#x20;

Then use the **tree** command to verify what happened.&#x20;

Empty directories were ignored and there were no files in any of the backup directories.&#x20;

We could use some of the switches in **xcopy** to make life easier. Try the command **xcopy .\CLI .\CLI3 /E /I /F** and use the command **tree** to ensure it worked.&#x20;

There is a more modern command called **robocopy** which is much more appropriate for use over a network on a modern system. Using help, figure out how to create a directory **CLI4** with all the subdirectories and files within.&#x20;

Now clean up the mess; delete the directories you have created.
