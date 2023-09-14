---
title: "How to read input from console in TCL"
date: "2016-01-31"
categories: 
  - "tcl"
---

You might know, we can use puts to write to console like this:

\[cpp\] puts "Hello world !" \[/cpp\]

In this post we will see how to read keyboard input from console using TCL script. Some time we need to take input from user to proceed further, for example adding two numbers. Here is syntax to read : **gets _channel\_ID_ _variable\_Name_**

Here, _channel\_ID_ is id of channel . It specify from where we have to read. To read from console we need to use **stdin** (standard input) as channel ID.

**variable\_Name** is name of variable where we have to store that text.

Let us check one sample example.

\[cpp\] puts "what is your favourite colour ?" gets stdin name\_of\_colour puts "Colour is $name\_of\_colour" \[/cpp\]

Output :

C:\\Tcl\\bin>tclsh inputDemo.tcl what is your favourite colour ? red Colour is red

Here is another example to add two numbers entered by user :

\[cpp\] puts "Enter first number for addition:" gets stdin first\_number

puts "Enter second number for addition:" gets stdin second\_number

set answer \[expr $first\_number + $second\_number\]

puts "Addition of $first\_number and $second\_number is : $answer" \[/cpp\]

 

Output will be :

C:\\Tcl\\bin>tclsh addition.tcl

Enter first number for addition: 33 Enter second number for addition: 11 Addition of 33 and 11 is : 44
