---
description: Finding your way around this document
---

# Introduction

I first started working with computer equipment back in the 1970s. My school got an Apple II, one of my neighbors got a Commodore VIC20 (look them up) and I got a book on programming from a friend. A few years later, I got to work on some of the early business computers, the first MAC and the most early business computers running an operating system called CPM. To operate these computers, with one or two floppy disk drives, required the ability to learn a disk operating system (DOS). It may sound bizarre, but the commands and approaches learned back then, are almost exactly the same as we use at the command prompt in a modern Windows computer.&#x20;

As I worked with larger computers in the 1980s, I began to work with the Unix command shell. Once again, nothing much has changed in the intervening years!

Before launching into more modern paradigms, we need to begin with the basic command prompt instructions. This technology may seem archaic, but it hasn’t gone away.&#x20;

We need to be able to work at the command prompt for some tasks, in Windows, Unix of any form, or on appliances and communications equipment. Until the 1980s, computers were primarily operated via text commands. Two operating systems common since this time are still in use today. DOS (now Windows) and Unix (most commonly, OS X, Linux, or BSD). In this document, I’m going to call the two environments Unix and DOS for simplicity. The structure of both systems is similar in many ways, however there are subtle differences. Although both operating systems have modern graphical user interfaces (GUI), many tasks require the administrator to be able to manipulate the operating system from the command prompt. For this reason, we will examine basic commands and directory structures in both operating systems.&#x20;

In DOS, we have a command processor. It may be a little more complex under Windows, but in pure DOS we have a programme called COMMAND.COM which interprets many of the basic commands. In Windows, we open a special command window to access the prompt.&#x20;

In UNIX we call this the Shell. The shell acts as an interface between the user and the kernel. When a user logs in, the login program checks the username and password, and then starts another program called the shell. The shell is a command line interpreter (CLI). It interprets the commands the user types in and arranges for them to be carried out.&#x20;

In our UNIX examples, we use the bash shell, however there are many others in common use including the Bourne Shell and the C Shell. Each command at the command prompt refers to a programme or routine within the operating system. With some commands it is possible to include parameters after the command, these are referred to as arguments.&#x20;

When you type a command, you run that programme and when it terminates, the shell gives the user another prompt. A user can customize his/her own shell, and users can use different shells on the same machine. The shell keeps a list of the commands you have typed in. If you need to repeat a command, use the cursor keys to scroll up and down the list or type history for a list of previous commands.

In this document, there are several key terms. These will be _italicized_. You may need to look up these terms to get a full understanding of them. Commands are generally shown in **bold**.

In these notes:

I will assume your Windows home directory is&#x20;

**C:\Users\\**_**username**_**\OneDrive - Atlantic TU\IaC\Week1**

If you have a different path, adapt!

## Copyright

The content of these notes are (c) John ORaw 2024.&#x20;

I have tried to acknowledge and cite sources, if you think I have missed crediting someone else's work, please contact me at john.oraw@atu.ie

If you find errors in my notes or something has been superseded without me noticing, please let me know.
