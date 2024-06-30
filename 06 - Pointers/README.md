void pointer

void pointer is a pointer which has no associated data type with it

It can point to any data of any data type and can be typecasted to any type


```
int main() { 

	int n = 10; 
	void *ptr = &n; 
	
	printf("%d", *(int*)ptr); 
	return @;
}
```

use of void pointer

malloc and calloc function returns a void pointer. Due to this reason, they can allocate a memory for any type of data. 
Syntax: `void* malloc(size_t size);`

malloc and calloc are used to allocate memory at runtime

Null pointer
A NULL pointer is a pointer that does not point to any memory location. It represents an invalid memory location.


When a NULL value is assigned to a pointer, then the pointer is considered as NULL pointer.

EXAMPLE: 
```
int main() { 
	int *ptr = NULL; 
	return 0;
```
use of void pointer

It's used to initialize a pointer when that poiter isn't assigned any valid memory address yet

useful for handling errors when using malloc function

```
int main() { 
	int *ptr; 
	ptr = (int*)malloc(2*sizeof(int)); 
	if(ptr == NULL) 
		printf(“Memory could not be allocated”); 
	else 
		printf(“Memory allocated successfully”) ; 
	return 0;
}
```

The value of NULL is 0. We can either use NULL or O but this 0 is written in context of pointers and is not equivalent to the integer 0. 

Always initlazie pointer with NULL 
perform NULL check before dereferncing any pointer

Dangling pointer
A dangling pointer is a ponter which points to some non-existing memory location

example

```
int main()
{
	int *ptr = (int *)malloc(sizeof(int));
	
	// some code

	free(ptr)
	// now ptr is a dangling pointer
	ptr = NULL;
	// now it's a NULL pointer

}
```

```
#include <stdio.h> 

int* fun() 
{ 
	int num = 10; 
	return &num; 
} 

int main() 
{ 
	int *ptr = NULL; 
	ptr = fun(); 
	printf("%d", *ptr); 
	return 0;
}	
```
Output should be Segmentaion fault as `num` is a local variable that get destroyed after retruening from a function


Wild pointer
a pointer that is not initialized

These pointers usually point to some arbitrary memory location and may cause a program to crash or misbehave.

EXAMPLE: 

```
int main() 
{
	int *p; 
	*p = 10; 
	return 0;
}
```
Output is undefined

Avoid wild 

Initialize them with the address of a known variable.
EXAMPLE:

```
int main()
{
	int var = 10;
	int *p; 
	P= &var 
	return 0;
```

explicity allocate the memory and put the valves in the allocated memory.
Exampte: 
```
int main() 
{ 
	int *p = (int *)malloc(sizeof(int));
	*p = 10; 
	free(p); 
	return 0;
}
```

To be conitinud
https://www.youtube.com/watch?v=udfbq4M2Kfc&list=PLBlnK6fEyqRj9lld8sWIUNwlKfdUoPd1Y&index=19