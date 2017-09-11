---
title: Introduction to Computational Thinking
summary: "An introduction to computational thinking and its relevance to programming and broader life experience."
---

# {{ page.title }}
{{ page.summary }}



## What is computational thinking?
Remember the quote from Steve Jobs that we saw last week and in our introductory video?

> Everyone in this country should learn how to program a computer...  
> because it teaches you how to think. ~ Steve Jobs

The reason that he is saying programming teaches us to think, is because the *computational thinking* skills that we will develop as we learn to program will teach us to think in new ways.

- We will use creativity, critical reasoning and problem solving skills to discover and test solutions to large, open-ended problems.
- We will perform logical decision analysis to have our code behave correctly under different conditions and for different situations.
- We will use pattern analysis and recognition to generalize and identify common problem solutions.
- We will learn to take large programs and simplify them by breaking them down into smaller, more manageable pieces.
- We will manage complexity by learning to hide details behind a layer of abstraction.
- We will use modeling to simulate real world objects and data in our programs.

## Computational Thinking
So what is computational thinking?

> A process that generalizes a solution to open ended problems. Open-ended problems encourage full, meaningful answers based on multiple variables, which require using decomposition, data representation, generalization, modeling, and algorithms found in Computational Thinking. ~[Wikipedia](https://en.wikipedia.org/wiki/Computational_thinking)

More simply stated, it's a set of principles that can be applied to solving big, open-ended problems.

Computational thinking involves several core ideas or principles:

- generalization
- abstraction
- composition & decomposition
- creativity
- data representation and modeling
- algorithms

We will cover each of these as we go through the course.  For this module, we will discuss  the first three in a little more detail.

### Generalization
Generalization in programming works much the way it does in everyday life.  We learn to recognize patterns and then generalize them into ways of representing either data or behaviors.  Data is the objects or things that our programs work with, while behaviors are the things that the programs *do*.

For this modules, we will be focusing on the behaviors, or actions. The things that our programs do.

As an example, imagine someone making sandwiches for a school lunch.  Back in the day, I used to get simple sandwiches such as ham, turkey, chicken, or meatloaf (my rare favorite). My mom had a some pretty basic sandwich recipes:

1. Ham Sandwich:  Take a slice of bread, add 2 slices of ham, top it with another slice of bread.
2. Turkey Sandwich:  Take a slice of bread, add 2 slices of turkey, top it with another slice of bread.
3. Chicken Sandwich:  Take a slice of bread, add some bits of chicken, top it with another slice of bread.
4. Meatloaf Sandwich: Take a slice of bread, add 2 slices of meatloaf, top it with another slice of bread.

But if we look closely at these recipes and generalize, we can simply this into one generic sandwich recipe that can produce all four types of sandwiches.

Take a slice of bread, add __*some meat*__, and then top it with another slice of bread.  The meat can change, but the rest of the recipe is the same. If we were to *program* this recipe, the meat would be an input parameter to the sandwich __function__.

Functions are an important part of programming as they allow use to define our own commands - such as `make sandwich` - to extend a programming language.  We will learn more about functions in our lab.  In the lab we will look for a pattern in drawing different polygon shapes, and use the pattern to write a function that can draw any (regular) polygon that we want.  Even ones with so many sides, we won't know what to call them.

Generalization has many benefits.  By having a single generalized recipe or function for making sandwiches (or drawing polygons), we can reuse the same code. This not only means that we write less code, but that if we find a bug (a problem in the code) and need to fix it, we only have to do that in one place. It also makes it easy to update or enhance the code, for example to put cheese on the sandwiches or alter the kind of bread, as again you only need to change the code in one place, and can see the benefits all over.

There are however some drawbacks to generalization.  While patterns and categorizations sometimes fit, there are almost always exceptions.  The more exceptions we find, the more our generalizations break down or start becoming overly complex.

### Abstraction
Abstraction is another concept that works pretty much the same way in our everyday lives and in programming, though we might not recognize it at first.  

Think about abstract art for example. Here are two images of Bart, my beloved old man cat.  The first is an actual photograph, while the second is my Bart inspired *abstract* cat art.

How would you describe the differences between the two representations of a cat?

{% include img-small.html url="/assets/images/comp-thinking-1/bart.png"
   alt="Photo of the fluffy grey Bart cat. No bow tolerated by this cat."
%}

{% include img-small.html url="/assets/images/comp-thinking-1/abstract-cat.png"
   alt="Line sketch of a cat with ears, eyes, whiskers, heart shaped nose, and a cute bow."
%}

Here is another example to help solidify your concept of abstraction.  Imagine you want to send your friend to your favorite restaurant or cafe.  You'd probably draw them a map, right?

{% include img-small.html url="/assets/images/comp-thinking-1/map-to-keys.jpg"
   alt="Hand-drawn map to Keys showing some landmarks and key roads like Hwy 36, Snelling, Larpenteur, and Lexington."
%}

{% include img-small.html url="/assets/images/comp-thinking-1/google-map-to-keys.png"
   alt="Google map to Keys showing all the nearby streets & landmarks."
%}

Would you draw every single street in the area or all the landmarks on a map when giving directions? Of course not! So, why is that a bad idea?  

It's much easier to follow directions if there is less extraneous detail, right? If we added every cross-street or landmark to the hand-drawn map, the important details can easily become lost.  On the other hand, if you don't recognize and know where the streets on the hand-drawn map are, you'll never get to Keys. Just like with generalization, there are both benefits and drawbacks to abstraction, depending on your purpose and perspective.

So what is generalization?  We've been circling around this concept without really defining it.  Simply put, abstraction is a way to hide the unimportant details of the moment. We might think those details are important at a different point in time, but for now they are just added complexity that is in the way of a simpler concept or task.

> In computer science, abstraction is a technique for managing complexity of computer systems. It works by establishing a level of complexity on which a person interacts with the system, suppressing the more complex details below the current level. ~[Wikipedia](https://en.wikipedia.org/wiki/Abstraction_(software_engineering))

The *hidden* details are just put behind what we call a layer of __abstraction__. They are there if we need to see them, but conveniently hidden away when we don't need to care about the specifics.

Our earlier examples all dealt with *things*, objects or data.  But we can use abstraction for behaviors or functions as well.  Think about your car.  Do you need to know all of the details on how your engine works in order to drive your car?  No, we just need to know some basic high-level things like how to start the car (turn the key or push a button), the gas pedal is go, the brake is stop, the steering wheel turns the car right & left, etc.  

In fact if we did need to know all of those details, its easy to assume there would be a lot less drivers on the road. Removing the need to know and interact with all those engine & mechanical details is one of the reasons that driving now is so much more popular and accessible than it was when cars were first invented. Back then you really needed to know a lot more about how the car and engine functioned. Do you know why?  The cars were far less reliable and you often had to *fix* them a drive.

When the details are hidden behind a layer of abstraction, things are much simpler to use and understand. However when things don't work correctly or don't behave as expected, those details are often important in troubleshooting and making any needed repairs, fixes, or changes. This is can be a drawback of abstraction.


### Composition & Decomposition
The last two topics we will discuss together as they are really opposite sides of the same coin.  __Decomposition__ you might recognize from every day life as a process of breaking things down or taking them apart. The first things I think of are zombies and composting, though it certainly doesn't have to mean decay & rot. You might also think of the process of making something like a fancy dinner and break that down into smaller parts that can be tackled independently, like marinating meat or vegetables, making a salad dish, making a dessert, preparing something to drink, etc.

__Composition__ on the other hand is putting things together, like composing music, a poem, or dance.  Music is a nice example as many of you will recognize that songs often have verses that repeat with some variation and chorus or refrains that are repeated unchanged.  The verses and chorus/refrain are arranged and assembled together to build up the entire song.

In programming we often use functions for composition/decomposition. Which one you are doing is often just a matter of perspective.  We often start by breaking a problem down into smaller pieces (much like the fancy dinner example), and then create separate functions for all of the pieces.  We then use composition to put the functions together to assemble larger, and larger parts until finally the whole problem has been solved.

## Functions
Functions are one of the foundational pieces of programming in any language. They are also the common thread that winds through these three computational-thinking concepts. We use functions for generalization, abstraction, and composition/decomposition, and often are doing all three things at the same time.

We will be exploring this in more depth through the in-class lab and homework, so try to keep these ideas in mind as you are working through the assignments.  

### Good functions
So, what makes a good function?  In my mind, the most important thing, even more so than does it work right, is that it must have a clear, meaningful name.  I rate this above correct behavior, because if the name isn't clear, then it's likely that the expected behavior isn't clear either.  That means we can't really even tell what the function should do, much less if it is doing it right.  

> If you can’t have someone else tell you what the function does just by reading the name, it is not a good name!

In addition to having a good name, good functions:

- use input to provide generalized solutions
- hide unnecessary details, simplifying complex code or problems
- can be used & reused (without code changes) to create more complex functions & programs
