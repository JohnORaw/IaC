# Visual Studio Code

VSC is now available on Windows, Mac and Linux. Review the installation instructions at this [link](https://code.visualstudio.com/).

I'm going to assume that you are using Windows. Adapt these notes if you are using Mac or Linux.

Go to your **C:\Python** directory, if it does not exist, create it now. From there, type **code .**&#x20;

Careful, that is the word code, then a space, then a dot!

```
C:\Python>code .
```

VSC will now start using C:\Python as its project folder. Any settings for the project you are working on will also be stored in this directory. You may need to load the Python extension.&#x20;

Select **Extension**, then **Install**.

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

VSC will not know you want to programme in Python. Open the command palette by typing **\[ctrl]\[shift]\[p]** and type **python select interpreter** then click on it.

You will be offered whatever versions of Python or Conda you have installed. I have two versions installed, I recommend you select the version you installed earlier, for me that will be 3.10.

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

We need to create a first Python programme to test. Click **New File** and give it a sensible name. I used 18MAY22-1.py and then wrote a simple Hello World programme. To test it, I clicked Run.

<figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

For now, when you are writing code, save it in&#x20;

* Windows: C:\Python&#x20;
* Linux: \~/Python&#x20;

In a production environment, you will never save work in an ephemeral location, one where you can lose your work. For now, back up your work to your university OneDrive each evening when you finish. In a later session, I'll show you how to use GitHub.
