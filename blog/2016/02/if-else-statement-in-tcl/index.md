---
title: "If Else statement in TCL"
date: "2016-02-05"
categories: 
  - "tcl"
---

Like other programming language TCL also support decision making using control structure like if -else , switch. As you might know that everything is command in TCL, including if-else and switch.

if statement validate expression and if expression is true then, block of statement written under if statement is executed. Here is syntax of if else:

if {boolean\_expression} {
   \# This block will be executed if boolean expression is true
}

One sample program based on above syntax:

```tcl
set number 0

if { $number \== 0 } {

puts "Number is zero"

}
```

Here if $number value is zero then expression will return true and as value of expression is true, statement written under if block will be executed.

**Output :**

C:\\Tcl\\bin>tclsh if\_demo.tcl Number is zero

Lets check how can we use if-else statement. Syntax of if-else statement:

if { boolean\_expression } {
  \# If the boolean expression is true this block will get executed
} else {
  \# If the boolean expression is false this block will get executed
}

Simple program based on if-else condition to check whether number is positive or negative.

```tcl
set number 2

if { $number \> 0 } {

puts "Number is Positive"

} else {

puts "Number is Negative"

}
```

**Output is:**

C:\\Tcl\\bin>tclsh if\_else\_demo.tcl Number is Positive
