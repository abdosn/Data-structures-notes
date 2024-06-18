# 01 - Introduction to data structures

And in this presentation, I will 
introduce what data structure is,

and some real life examples of data structures.

# What is data ?

The better definition could be a dictionary definition.

> The quantities, characters or symbols on which operations are performed by a computer, which may be stored and transmitted in the form of electrical signals and recorded on magnetic, optical or mechanical recording media.

You can think of a data as 
quantities, characters or symbols

on which we can perform operations,

we can store them, we can transmit them

obviously in the form of electrical 
signals in our computer. Right?


Now, let's see one example here.

```
C = a + b
```

Here in this case, I am performing this

operation on these two data. Right?

We can think of these two as data

because we are performing operations on them.

These are just quantities. Right?

We can store them, transmit them.

So, they are satisfying the properties of data.

So, I can say that these are my data.

## when data becomes information ?

There is a distinction between data and an information.

And it is one such topic which is very confusing.

We often interchange these two terms. Right?

But there is a distinction between data and information.

Let's try to understand what is that.

When I say just collection 
of characters like this `NAMHAREL-DBA SI EMAN YM`

then this is just a data.

Because it is just a collection of characters.

I won't be able to understand it properly. Right?

But, when I process this data and let's say I reverse this whole string, means the last character becomes the first character, second last character becomes 
the second character and so on. `MY NAME IS ABD-ELRAHMAN`

Then it becomes an information. 

Because, now I can read this and I can understand what is written.

Here, I have written my name is Abdelrahman.

So, it is quite understandable.

So, I can say that now here, data becomes information

because I can extract some meaning from it.

So, if data is arranged in a systematic way, then it gets a structure and become meaningful.

Therefore, I can say that, this meaningful or processed data is called information.

Now, it is not difficult for us to understand that

the data needs to be managed in such a way so that it can produce some 
meaningful information.

We need to arrange our data, we need to manage out data in such a way so that we can produce some meaningful information.

To provide an appropriate way to structure the data, we need to 
know about data structures.

That is why, it is so useful to understand data structures.

Data structure gives us the way to structure the data, to appropriately manage the data, so that we can get some meaningful information from it.

And not only that, we can use it whenever required in an efficient way.

This is the reason, why companies are preferring this subject over other subjects because this is very important subject. Right?

# Data structure

> A data structure structure is the systematic way to organize data so that it can be used efficiently.

So, organizing the data in such a way so that we can use it efficiently is what data structure is all about.

We are arranging the data, we are organizing the data, we are managing the data in such a way so that we can use it efficiently.

When I say efficiency, I mean in terms of time as well as space.

Let's see one example of a classical data structure, ***Arrays***.

We have used it many number of times.

We can think of it as a sequence or collection of some symbols, characters, integers, floats, something like that. Right?

You can think of array as a data structure because it is helping us in managing 
the data in an appropriate way, *actually in a sequential manner*.

Now, here is an example, why this data structure is so useful.

Instead of creating multiple variables of same type,

why not create an array to store all the values?

Let's say, I need 100 integers. Why do I require to create 100 variables for 100 integers, when I can create a single array and store all the integers in them.

Isn't that so? That is why, arrays are so useful.

Or you can think of one example like storing strings.

You know that strings are nothing but sequence of characters. Right?

Let's say, a string consist of 100 such characters.

Now, are you going to create 100 variables for that?

No, you can create one array which can store that whole string.

And we would be able to access it very easily. Isn't that so?

So, this requires array and that is why we need arrays.

Because it helps us in managing our data in an appropriate way.

That is why, it is a very useful data structure for us.

Now, let's discuss some real life examples of data structures to help understand, 

why do we need data structures.

Here is an example.

Did you know that stack data structure is used in implementing redo and undo feature?

You know, this is the famous feature which we are using many number 
of times in our applications. Right?

One such application is Google docs, or power point, or Microsoft word.

Redo and undo feature is very famous.

But, did you know that stack data structure is used in implementing this feature?

Let's see how?

Here, I have taken an interface of Google docs.

Here, I am going to write something.

Let's say, I have written, "The primary goal of Neso Academy is to give quality edcation." 

I want to write education here, but I forgot to mention 'u' here.

So, instead I have written edcation, something like that.

Let me tell you that, here a stack is maintained where each and every information 
that I have entered gets stored.

Like in this case, 'quality' is stored, 'ed' is stored separately, 'cation' is stored separately.

So, this is our undo stack.

Okay, we know that, in stack, the data is

placed from top and whenever we want to get the data, we can get it from the top.

We can access only the top element.

Right? Now, when I press control z,

then I know, it means undo. Right?

So, what it does is, it selects the top element and it pops that element out of the stack and places it in the redo stack.

That is why, we can see here, that 'cation' gets removed when I press control z. Control z means, undo the operation which I have performed.

Here, in this case, I have entered cation. I just can remove that out of the stack and then after that, that particular element will get placed with in this redo stack.

Why it is placed in this another stack?

Because, when I press control y, that is redo then we can get that again.

That is, this cation -- I would be able to get that again over here.

May be I want to redo my operation, that is why, redo stack is also required.

Now, I can continue writing.

I have written, "The primary goal of Neso Academy is to give quality education to" --actually, I want to write everyone but accidentally, I have written 'ebery' instead of every.

I press control z, this element gets selected and you know, it will get poped out of the stack and will get placed within this redo stack.

And you can see here, the operation here is undone. Right?

Now, let's say, I want to redo the operation.

When I click on control y, then this particular element get selected and it will get poped out of the stack and will get pushed within this undo stack once again.

So, here the operation is redone.

This is how undo redo feature works.

And this is one such application of data structures.

And you can see here, stack is our data structure.

Now, let's see another example.

Which data structure is used to store an image as a bitmap?

Do you know which data structure is used to

store an image as a bitmap?

There are two types of images, 
bitmap images and vector images.

Now, when I talk about a bitmap image, you know which data structure 
is used to store that image?

Guess what, it is an array.

Array is so useful that, it is used in storing an image as well.

Let's see, how?

Bitmap images are stored as a series of tiny dots called pixels.

Right?

So, here you can see in this image, 

that these tiny dots or squares are called as pixels.

Here each pixel is actually a small square that is assigned a color and then arranged in a pattern to form an image like the following.

So, you can think of a two dimensional array like this.

Here, in this example it is 37 cross 40.

Now, within that two dimensional array, 

you are storing pixel information, that is

each pixel color you are storing

and then after that, you are 
arranging it in a systematic way

and finally we get this as a result,

that is an image of a Pikachu. Right?

So, a two dimensional array of size 37 cross 40

is enough to store this image. Isn't that so?

Now, let's see our example number three.

Storing the friendship information 
on a social networking site.

Do you know how Facebook is 
storing the information of friends?

Let's see an example here.

Let's say, James is a friend of Mark.

Not only that, James is friend with Lia as well.

So, here we are maintaining 
the connections between them

This particular edge is representing

the relationship between James and Mark. Okay.

Similarly, James is friend with Lia,

and it is represented by this edge.

Not only that, Lucy is friend 
with both Mark as well as Lia.

So here, I am maintaining the connections like this.

But it should be noted that, 
James and Lucy are not friends.

That's why there is no edge between them.

You can guess that, which data structure 

is used to store this information.

It is graph.

We can use graph data structure 
to store information like this.

And now, you can understand why 
data structures are so important.

They are useful in day to day life

and we using them more frequently and that is why,

it is so hot in IT industry.

Okay friends, this is it for now.

Thank you for watching this presentation.

