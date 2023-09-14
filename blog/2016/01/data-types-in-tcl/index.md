---
title: "Data Types in TCL"
date: "2016-01-26"
categories: 
  - "tcl"
---

TCL stores value as Object and every object having String representation and It may have secondary representation if needed.

Let me explain when this secondary represenation is used. For example you assign value to variable like this :

\[cpp\]set a 5\[/cpp\]

TCl will create variable 'a' and assign 5 as string value . Now if you use variable 'a' where value of 'a' will be require as integer (for example arithmetic operations) then TCL will translate the string 5 into integer value. Value of 5 will remain integer until it is required as a string. Check following script and its comments for more detail.

\[cpp\] set a 5 ; # a as string

set a \[expr $a+4\] ; # a as integer

puts $a ; # a as string

\[/cpp\]

See how can we use float value with TCL script .

\[cpp\]

set a 4.2

set a \[expr $a+0.2\]

puts $a ;# will print 4.4

\[/cpp\]

**List** List is basically string separated with whitespace . Curly braces or double quotes can be used to represent List.  

\[cpp\]

set listOfDay {monday tuesday wednesday}

puts $listOfDay ; # output => monday tuesday wednesday

set listOfOdd { 3 5 7 }

puts $listOfOdd ; # outout => 3 5 7

<b>\[/cpp\]

**Associative Array**

Associative arrays are like Key Value pair. Key can be string value .

\[cpp\]

set name(IN) "India" set name(UK) "United Kingdom"

puts "Countries : $name(IN) $name(UK)"

\# Output=> Countries : India United Kingdom

\[/cpp\]
