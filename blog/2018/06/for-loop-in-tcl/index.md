---
title: "For loop in TCL"
date: "2018-06-27"
categories: 
  - "tcl"
---

For loop in TCL can be achieved using the command **for**. It is used to execute code for multiple numbers of time.

Let's see the syntax of **for** command:

```tcl
for { start } { test } { next }

{

body

}

```

Here, **start** portion is used to initialise the variable. **test** is an expression, which will return either true or false . **next** is the portion to increment a variable, which has been written in the start portion.

Let's see some examples:

1. Increment by 1

```tcl

# Example for loop

for {set i 0} {$i < 3} {incr i} {

puts "Value of i is: $i"

}

```

Output is :

```tcl

Value of i is: 0 
Value of i is: 1 
Value of i is: 2

```

 

2\. Increment by 2

```tcl

# Example increment by 2

for {set i 0} {$i < 5} {incr i 2} {

puts "Value of i is: $i"

}

```

Output :

```tcl

Value of i is: 0
Value of i is: 2
Value of i is: 4

```

 

3\. Loop through in reverse direction:

```tcl

# Loop through in reverse direction

for {set i 5} {$i > 0} {incr i -1} {

puts "Value of i is: $i"

}

```

Output:

```tcl

Value of i is: 5
Value of i is: 4
Value of i is: 3
Value of i is: 2
Value of i is: 1

```
