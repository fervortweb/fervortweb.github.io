---
title: "How to read input from console in TCL"
date: "2016-01-31"
categories: 
  - "tcl"
---

You might know, we can use puts to write to console like this:

```tcl
puts "Hello world !"
```

In this post we will see how to read keyboard input from console using TCL script. Some time we need to take input from user to proceed further, for example adding two numbers. Here is syntax to read : **gets _channel\_ID_ _variable\_Name_**

Here, _channel\_ID_ is id of channel . It specify from where we have to read. To read from console we need to use **stdin** (standard input) as channel ID.

**variable\_Name** is name of variable where we have to store that text.

Let us check one sample example.

```tcl
puts "what is your favourite colour ?" gets stdin name_of_colour puts "Colour is $name_of_colour"
```

Output :

C:\\Tcl\\bin>tclsh inputDemo.tcl what is your favourite colour ? red Colour is red

Here is another example to add two numbers entered by user :

```tcl
puts "Enter first number for addition:" gets stdin first_number

puts "Enter second number for addition:" gets stdin second_number

set answer [expr $first_number + $second_number]

puts "Addition of $first_number and $second_number is : $answer"

```

 

Output will be :

C:\\Tcl\\bin>tclsh addition.tcl

Enter first number for addition: 33 Enter second number for addition: 11 Addition of 33 and 11 is : 44
