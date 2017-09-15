---
title: Process Flow
summary: "Flow charts are often used to document and describe processes both in business and in programming. So let's learn to use them."
---

# {{ page.title }}
{{ page.summary }}



## Basic Structures
There are 3 basic structures in programming & more general process flows:

- sequences
- choices (decisions or branches)
- iteration (loops or repetition)

In the earlier modules, we used two of the three - sequences and iteration - in our program code.  In this module, we will introduce the third, choices. In this reading, we will examine each of these structures and how they are used in process flows.

## Sequences
The flowchart shown below illustrates a simple sequence.  A __sequence__ is just a series of commands that are performed in order.

{% include img-medium.html url="/assets/images/flow-charting/simple-3step-sequence.png"
   alt="Flowchart showing a simple sequences: start, followed by 3 steps, & end."
%}

The flowchart proceeds from the start to the end, following the connections between steps in the direction of the arrows.  The two flowcharts below represent the same process:

{% include img-medium.html url="/assets/images/flow-charting/simple-sequence.png"
   alt="Flowchart showing simple sequences, illustrating that they may be shown in any order and that following the arrows is important."
%}

It is important to pay attention to the arrows that join the steps together, as the flowchart. The flowchart may not always read right to left or top to bottom.  

## Choices
There are often times where we only want to perform certain actions under certain conditions.  For example, we might want to take our rain gear if the weather forecast predicts rain, but we'll leave it at home if it does not.  We can show this in our flowcharts using choices. A __choice__ is simply a decision point in our process, where the path we follow next is determined by some condition or criteria.

Here is a simple flowchart with a choice illustrating the above example.
{% include img-small.html url="/assets/images/flow-charting/check-weather.png"
   alt="Flowchart with a choice illustrating the example above."
%}

You will often hear this said using the key words *if* and *then*. For example:
__If__ it is going to rain, __then__ we pick up rain gear.

This can be worded with a negative as well, with no change in the meaning:
__If__ it is __not__ going to rain, __then__ we do nothing.

With the negative wording, it can be said we do *nothing* as both paths join back together before going on to the next step to leave the house.  There is nothing *special* that we do only when it is not expected to rain.  

In many cases we are making a choice between two different actions based on a condition or criteria. For example we go to work during the week and do something fun on the weekend.

{% include img-small.html url="/assets/images/flow-charting/weekend.png"
   alt="Flowchart with a choice illustrating the example above."
%}

In business processes, choices may be represented as any sort of question.  However when writing flowcharts for programming problems, you should always word your choice as a yes or no question.  This allows your process to be more easily translated into code.


## Iteration
Many processes include steps that might be repeated.  For example in last week's lab we were drawing shapes and repeating a sequence of move and turn for each side on our shape.  To draw a square, the move and turn sequence was repeated 4 times.  This repetition of steps is called a loop or __iteration__.

The following are three example flowcharts that contain an iteration or loop.

{% include img-medium.html url="/assets/images/flow-charting/simple-loops.png"
   alt="Flowchart showing simple iterations. Examples discussed below."
%}

Note that an iteration is *always* controlled by a choice that indicates whether we should repeat or not.  With loops, instead of wording the choice with an if, we often read it using the words __until__ or __while__.

### First example
In the first example, we are waiting. There are no steps shown in the loop. Although we might have included a step that says "wait", that is often considered understood and omitted.

- Start
- Pour hot water over coffee grounds.
- __Until__ 5 minutes have passed:
  - (implicit wait)
- Press the plunger on the coffee pot.
- End

### Second Example
The second example is similar to the first, except now we have explicitly shown that certain steps are occurring in the loop.

- Start
- Wake-up
- __Until__ it is time to get out of bed:
  - Go back to sleep
  - Wake-up (step is *potentially* repeated)
- Get out of bed
- End

In this example, we must wake-up to determine if it is time to get out of bed, so it is necessary to repeat that step before and inside of the loop.

### Third example
The last example comes from those shampoo bottles with the rinse and repeat.

- Start
- Wet hair
- __Until__ we have shampooed twice:
  - shampoo hair
  - rinse out shampoo
- End

Notice in the flow chart, the choice is shown at the bottom, but we could also have moved the choice higher in the process (as shown in the description above) without changing the overall behavior.  This prevents us from needing to write the shampoo and rinse steps both outside and inside the loop.  

It's often possible to move the choice before the steps to repeat.  Watch for this and try to design the flowcharts that way as it will more naturally fit your program code.

## Larger "Steps"
If you shift your perspective a bit, you can think of choices and iterations as just being another *larger* and more complicated step in the overall program sequence.  

{% include img-medium.html url="/assets/images/flow-charting/perspective.png"
   alt="Same flowcharts from above, highlighting choices & iterations as single steps in the larger process."
%}

This ties nicely into how these structures are represented in Snap! and other programming languages.  In Snap! choices and iterations are represented by a single block that surrounds other blocks.  In other programming languages, the structure are very similar and they also contain what we call *blocks* of code.

{% include img-small.html url="/assets/images/flow-charting/draw_square_repeat.png"
   alt="Snap block showing repeat drawing sides of a square."
%}
