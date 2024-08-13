# Directories and File Structures

Directories would be hard to use if you didn't know which one you were working in!! The directory we are currently in is called the _working directory_ or sometime the _current directory_. We have previously seen how to tell what directory we are in, both in Unix and in DOS. Now we know where we are the next requirement is to see what files are there.&#x20;

In a DOS command window, type **c:\users\\**_**username**_**\IaC\Week1** to change your working directory, or **C:\users\\**_**Username**_**\IaC\Week1** if you are working on a home computer.

**dir** to get a basic directory listing. In the third column, you may see the text \<DIR>. Any such entry refers to a subdirectory which may contain other files and directories. A directory under another directory is referred to as a sub-directory.&#x20;

**dir /p** to get a paginated directory, useful when there are very many files

**dir /a** to show hidden files&#x20;

**dir /w** to show files in a wide format&#x20;

**dir /?** to get a list of all options&#x20;

Depending on your OS and how you are viewing it, some of the directory listing shows file names in various colors.&#x20;

In either DOS or Unix

(.) means the current directory, so typing **cd .** means stay where you are.&#x20;

(..) means the parent of the current directory, so typing **cd ..** will take you one directory up the hierarchy. These become very important later!!&#x20;

For completeness, I should comment that this overview is simplified. Files may be multi-dimensional; they may have other _streams_ apart from the one holding the data. Do an Internet search on NTFS streams to see what I mean.
