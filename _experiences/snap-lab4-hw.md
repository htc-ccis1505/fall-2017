---
title: Snap Lab 4 - Homework
summary: "This lab contains problems similar to those that will be found on the first exam."
---

# {{ page.title }}
{{ page. summary }}

## Introduction
The HW lab is intended to build on and further develop the skills you learned in the in-class lab as well as review and pull together all of the concepts we have learned to date.

When you are done with all of the problems on this worksheet, export them as one single Snap XML file to submit to the assignment box on D2L.

If you have forgotten how to export your code, you can refer back to [Lab 1: An Introduction to Snap!](https://htc-ccis1505.github.io/main-labs/cur-new/programming/snap-intro/save-and-share.html?topic=htc_fund%2Fintro%2F1-introduction-short.topic&course=htc_f17.html).

## Assignment
For this lab, no script is required to run when the “green flag” is clicked, but please ensure all custom blocks made are well named, easy to find, and shown on the “Scripts” tab.  Include multiple copies of each block on the “Scripts” tab to show that you have tested it with “good” test data values.

### Same Loop 3-Ways!
Create a command block that will use a repeat loop to count from 1 to a some max number. (The max number to count up to should be an input parameter on the block. To do the counting, just have the sprite say each number for 1 second.)

1. Create a command block that will use a repeat-until loop to do the same thing, count from 1 up to some max number.

2. Create a command block that will use a for loop to count from 1 number to do the same thing, count from 1 up to some max number.

__Challenge:__ Create 3 similar blocks but have them count by 2.  This is a little more tricky!  You can’t change the counter in a for loop. Can you think of another way to skip a number?  


### Fun With Predicates
Remember predicates should report (or return) only Boolean values - true or false.

1. Make a block to determine if a number is negative (less than zero).  

2. Make a block to determine if a string contains a certain letter. (Use input parameters for both the string and the letter.)

3. Make a block to determine if a string contains less than some number of characters.  (Use input parameters for both values.)


### Fun With Reporters
Remember to check that your reporter always reports a value.  

{% include alert.html type="tip"
    content="Remember to use decomposition to break down complex problems.  Two of these problems need to know if a letter is a vowel.  Making a block for just that part of the problem first will allow you to simplify those larger problems." %}

1. Make a block to count the number of vowels in a string.  Make a block to count the number of consonants.

2. Make a block to replace all the vowels in a string with an asterisk \*.

3. Make a block to reverse a string.  For example if the input string is “hello”, the output (or reported value) should be “olleh”.
