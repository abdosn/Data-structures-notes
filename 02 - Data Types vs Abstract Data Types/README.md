# 02 - Data Types vs Abstract Data Types

# What is a data type?


There are two important things about data type

1. It defines a certain domain of values.

2. It defines operations allowed on those values.

Example : integer 

1. Can take only integer values.               

2. The operations allowed are addition, subtraction, multiplication, bitwise operations etc.

We can perform almost every operation with integer type.

Example: Float

1. Takes only floating point values.

2. The operations allowed are addition, subtraction, multiplication, division **BUT** we cannot perform bitwise and mod (%) operations on them.

# User-defined datatype


You already know primitive data types like integer, character, float. Right?

But there is a concept of user defined data type which we should also know.

> The operations and values of user defined data types are not specified in the language itself, but is specified by the user.

Examples: Structure, union and enumeration 

For example, 
```
struct point{
int x;
int y;
};
```
we have combined these two integers to form a new type, that is point.

So, it's a user defined data type.
# Abstract Data Types (ADT)

ADTs or Abstract data types are like user defined data types which defines operations on values using functions without specifying what is there inside the function and how the operations are performed.

First of all, we are defining operations, that is true.

But we are defining operations on values, that is also true, using functions.

It should be well noted that, we are defining operations using functions, without specifying what is there inside the function.

And we are not specifying anything inside, what is there inside the function. Okay, and how the operations are performed.

Let's take an example of a stack ADT.

A stack consists of elements of same type arranged in a sequential order.

So, what types of elements are allowed in a stack?

The elements of same type.

And that too, they are arranged in a sequential order, 

we already know that right?

Now, the operations allowed on them could be

initialize- we can define an initialize 
function which initializes the stack

to be empty actually. We can 
perform a push operation

that is, insert an element into the stack.

We can perform pop operation that is, 
delete an element from the stack.

We can check is stack empty or

we can check is stack full.

So, these are the operations which we can 
define and we can perform on stack.

These are functions, as you can see.

Here, we are specifying function but

we are not saying anything, 
how they can be implemented.

We are just specifying them.

That is called abstract data type.

We know that, what type of elements are allowed

and we also know that what operations

we can perform, but we don't 
know what is there inside. Okay.

Think of ADT as a black box which hides 

the inner structure and design 
of the data type from the user.

We can think of it like, it hides all

the implementation details from us.

This is very important which 
we will understand later.

There are multiple ways to implement an ADT.

Let me tell you, this is very important.

There are multiple ways to implement an ADT.

For example, a stack ADT can be 
implemented using arrays or linked lists.

It should be well noted that 
stack itself is a data structure,

we can implement this data structure using

other data structures like arrays or linked lists.

Okay. So, a stack ADT, which we 
know is right now is a skeleton,

can be implemented using arrays or linked lists.

Now, the question that immediately arises

that why do we even need ADTs?

Why do we need skeletons?

Why can't we simply implement things, 
you know display it to the user.

Why ADT?

Before moving further, we should 
understand some terminology.

The program which uses data 
structure is called a client program.

You should note this very clearly,

that the program which uses data structure

is called a client program. It has access to the ADT

that is the interface, nothing else. Just abstract.

And the program which implements the 

data structure is known as the implementation.

So, we have two programs, one is client program,

the other one is implementation.

Implementation is the one which implements the

data structure and the client program is the one

which just uses the interface, that is the 
outside details, nothing inside. Okay.

Now, let's discuss the advantage.

Let's say, if someone wants to use the stack

in the program, then he can simply use

push and pop operations without 
knowing its implementation.

A user doesn't have to worry about

how the operations are performed.

Okay. If someone wants to use the stack program,

we know that, program which uses the data structure

is called the client program.

It has access to the interface only

and nothing inside. So, he can 
simply use push and pop operations

without knowing its implementation.

Apart from this, if in future, the implementation

of stack is changed from array to linked list,

let's say, previously the stack 
was implemented using arrays,

right? But know, let's say it is changed to linked list.

Then the client program will work in the 

same way without being affected.

There is nothing to discuss with client program.

Client program has nothing to do with it.

It can simply use the interface,

without knowing what is going on inside.

So, if the implementation is 
changed from array to linked list,

nothing will be affected in the client program.

This is one of the biggest advantages 
of using abstract data types.

Now, it should be clear that, why we are using it.

Because, with the help of abstract data types,

we are actually separating the two worlds.

We are just providing the user, an interface.

The rest of the details, 
the implementation part

is done in the back end.

User doesn't have to worry about it.

The implementation can go on

without affecting the client program.

That is why, the need of abstract data type came.

Now, here is the conclusion of this lecture.

Abstract data type provides abstraction.

We should understand this, 
that abstract data type

provides abstraction 
which means hiding details

from the user and it is very important because

user doesn't bother about how that particular

thing is implemented. He just 
have to use that thing.

That's it. So, this separation is required.

That's why abstract data type 
is very useful concept. 

Okay friends, this is it for now.

Thank you for watching this presentation.

