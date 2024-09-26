# Linux in Windows

You can do this activity on a home computer to allow you to work with Linux easily. This will also work in Azure Labs.&#x20;

**Do not try this in a University Laboratory**.

**Do not use this if you plan to use VMWare Workstation.**

Some terminology is important. The physical computer is the _host_. Any Linux instance we run under the host operating system is a _Virtual Machine_ (VM).

Some years ago, Microsoft introduced the [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/about) (WSL). At the time, I was not impressed and thought it was a kludge. But WSL2 is now settled and has some maturity and allows us the ability to install a useful operating system like Ubuntu as a Virtual Machine (VM). And we can do this on any Windows 10/11 computer with a few button ticks.

Note that you must have Windows 10 v.2004 or better (2020) to install WSL2.

Open **Turn Windows Features on or off**

Enable the&#x20;

* Windows Subsystem for Linux
* Windows Virtual Machine Platform

Click **OK** and reboot the computer.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

After the reboot, the extra software is installed.

Now go to the **Microsoft** **Store** and search for **Ubuntu**. I recommend you use Ubuntu 22.04 LTS

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

Install and open. In 2023 I got the error as shown. Testing in August 2024, no error!

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

In 2023, I used the suggested link and downloaded **wsl\_update\_x64.msi** and ran it.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

I then run Ubuntu as an app.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>
