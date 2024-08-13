# Runtime Environments

There is a completely different approach that we could take to programming. It's clearly most efficient to right in a high-level language. But best performance comes from using compiled code.&#x20;

Some languages take benefit from both of these approaches. We have a large piece of code called a runtime environment. The high-level language calls highly optimized machine code in this runtime environment.

## Java

Java was written as an improvement to C. C handles memory management in such a manual way, it tends to lead to buggy code.&#x20;

Java source code is compiled into _bytecode_, which runs on a _Java Virtual Machine_ (JVM). The JVM is called virtual because it is an abstract computer defined by a specification, it may be software on top of an operating system, or hardware, or any mixture of the two. Java source code can run on any platform for which a JVM is available.

On each platform, the JVM can be written in an efficient language like C. In many respects, the JVM is exactly like a CPU, with mnemonics and opcodes, stack and heap and its job is similar; to load class files and execute the Java byte code within them.

```
class howaya { 
	public static void main(String args[]){ 
		System.out.println("Hello World!"); 
	}	 
}

```

Any platform which implements the JVM can run the bytecode making it (mostly!) platform independent. This is called _Write Once, Run Anywhere_ (WORA). There are ways to run Java without the performance impact of the JVM.

## .Net

Microsoft took the same sort of approach when they introduced .Net. Recently, Microsoft has made .Net available for Linux.

## Python

Earlier I said that Python was an interpreted programming language. Once you categorize things, you do fail to catch the full picture. Python compiles source code into a byte code intended for a virtual machine, just like Java. When you're working with Python, you will notice **.pyc** files, this is the compiled _bytecode_.&#x20;

I write a simple Hello World program.

```
print("Hello World")
```

I manually compile it on a Windows machine.

```
C:\Users\John.ORaw>python
Python 3.10.5 (tags/v3.10.5:f377153, Jun  6 2022, 16:14:13) [MSC v.1929 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> import py_compile
>>> py_compile.compile('hello.py')
'__pycache__\\hello.cpython-310.pyc'
>>> quit()

```

I then examine the **.pyc** file using the hex viewer plugin in Notepad++.

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Every byte has meaning. I found a good pyc [decoder](https://github.com/nedbat/coveragepy/blob/master/lab/show\_pyc.py) on GITHUB and got the following output.

```
magic b'6f0d0d0a'
flags 0x00000000
moddate b'dcf00965' (Tue Sep 19 20:05:00 2023)
pysize b'16000000' (22)
code
    name '<module>'
    argcount 0
    nlocals 0
    stacksize 2
    flags 0040: CO_NOFREE
    code 650064008301010064015300
  1           0 LOAD_NAME                0 (print)
              2 LOAD_CONST               0 ('Hello World')
              4 CALL_FUNCTION            1
              6 POP_TOP
              8 LOAD_CONST               1 (None)
             10 RETURN_VALUE
    consts
        0: 'Hello World'
        1: None
    names ('print',)
    varnames ()
    freevars ()
    cellvars ()
    filename 'hello.py'
    firstlineno 1
    lnotab
        1:0
    linetable 0c00
        co_lines 1:0-12
```

To me, this make perfect sense, but I have been messing with source code and object files since the later 1970s. We will not go much further into this here, if you do low level programming with me, we will!
