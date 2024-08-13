# Compiling

I use the gcc programme in Linux to compile the above file.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

In my example

```
gcc -c -O2 -Wa,-al hello.c 
```

* \-c tells gcc to compile or assemble source files, but not to link them
* \-O2 produces more fully optimized code
* \-Wa tells the compiler to pass the comma-separated list of options which follows it on to the assembler.
* The -al option is an assembler option to request an assembler listing.
