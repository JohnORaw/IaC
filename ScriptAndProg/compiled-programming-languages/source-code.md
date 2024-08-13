# Source Code

Originally, I wrote C programs in a Unix text editor like ed or vi. The Include directive allowed me to add code to a programme or was used to specify a library to use.

```
#include <stdio.h> 
int a, c; 

static void rubbish (int b) 
{ c = a + b; 
printf ("%d + %d = %d\n", a, b, c); 
} 

int main (void) { 
int b; 
a = 3; 
b = 4; 
printf ("Hello, world!\n"); 
rubbish (b); 
return 0;

```

