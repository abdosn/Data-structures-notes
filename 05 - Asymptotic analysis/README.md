Efficiency of data structures is always measured in terms of Time and space.


An ideal data structure could be the one that takes the least possible time for all its operations and consumes the least memory space.

on what basis we could comapre the time complexity of the data structures

operatins peroformed


example 
to add data at the begining of an array
how
by shifting all elemnts to the right 
then there will be a postion free at the begining

in linked list 
the operation is peroformed by detaching head to our node

so inserting an element to the begining of data structres is faster in the case of linked list than an array

time complextiy of operations depends on the size of data to be processed
in other words time complexxity is a function in size

Big O notation

big o notaion is ussed to measure the performance of any algortih by providing the ordre of growwth of function

it gives the upper bound on a function by which we can make sure that the function wll never grow faster than this upper bound

Gives us an approximate runtime of the operationds perfomred on data streuctrues

```
int main() 
{  
	int i, sum = 0, n; // --> 1 time
	scanf("%d", &n);  // --> 1 time
	for(i=1; i<=n; i++) 
	{ 
		sum = sum + i; // --> n times
	} 
	printf("%d", sum); // --> 1 time
	return 0; // --> 1 time
}
```
The worst case time comlexity is O(n)
it means that the time is linear with n (Linear growth)

This code calclated numbers between 1 and n

```
int main() 
{ 
	int i, sum = 0, n; // --> 1 time
	scanf("%d", &n); // --> 1 time
	printf("%d", n*(n+1)/2); // --> 1 time
	return 0; // --> 1 time
}
```
The above code do the same task but its time comlexity is O(1)
it means time does not depend on n (Constant growth)


Guidelines

Loops
Loops executes n times
```
for( i = 1  ; i <= n ; i++)
// statement
```
Total Time = O(n)

Nested loop
```
for( i = 1  ; i <= n ; i++){
	for( j = 1  ; i <= n ; i++){
		// statement
	}

}
```


| i = 1      | i = 2      | i = 3      | i = 4      | ... |
| ---------- | ---------- | ---------- | ---------- | --- |
| j = 1 to n | j = 1 to n | j = 1 to n | j = 1 to n |     |

Outer loop executes n times and inner loop executes n times

Total Time = O(n\*n)

Consecutive statements

```
int x = 2; // 1 time
int i; // 1 time
x = + 1; // 1 time
for(i=1; i<x=n; i++) { // n times 
	//statement 
} 

for(i = 1; i<x=n; i++) { // n*n time
	for(j = 1; j<=n; j++) { 
		//statement 
		}
}
```

Total Time = n\*n + n + 3 = O(n\*n) 

Conditions
```
scanf(“%d”, &n);
if (n == 0) { 
	//statement 
} 
else { 
	for(i=1; i<=n; i++) 
		//statement
}

```
if n = 0 then Total time = O(1)

else them Total time = O(n)

so the total time of code is O(n) *The worst case scenario*

```
for(i=1 ; i<=n ; )
{
	//statement
	i = i*2;
}

```


| Iteration 1   | Iteration 2   | Iteration 3   | Iteration 4   | Iteration 5    | Iteration k     |
| ------------- | ------------- | ------------- | ------------- | -------------- | --------------- |
| i = 1 - *2^0* | i = 2 - *2^1* | i = 4 - *2^2* | i = 8 - *2^3* | i = 16 - *2^4* | i = n - *2^k-1* |
$$
n = 2^{k-1}
$$
$$
k-1 = log_{2}n
$$
$$
k = log_2n + 1
$$
Then the Total time = O(log_2n)

```
for(i=n; i>=1; ) 
{ 
	//statement 
	i = i/2;
}

```
the Total time = O(log_2n)

What is the time complexity of the following program?  
```
void fun(int n) { 
	int i,j, k, count = 0; 
	for(i = n/2; i <= n; i++)
		for(j = 1; j+n/2 <= n; j++)
			for(k = 1; k <= n; k = k*2) 
				count++;
}
```

What is the time complexity of the following program?  
```
void fun(int n) { 
	if(n <= 1) return; 
	int i, j; 
	for(i=1; i<=n; i++) 
		for(j=1; j<=nj j++) { 
			printf (“Hello\n”) ; 
			break;
		}
}

```

What is the time complexity of the following program?  
```
void fun(int n) { 
	int i,j; 
	for(i=1; i<=n/3; i++) 
		for(j=1; j<=n; j += 4) 
			printf(“Hello\n”);
}

```