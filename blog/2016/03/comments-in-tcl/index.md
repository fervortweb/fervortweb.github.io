---
title: "Comments in TCL"
date: "2016-03-24"
categories: 
  - "tcl"
---

We are  adding comments in source code to make it easier to understand or we can also use comments to add legal notices, like copyrights or to add some TODOs, Author name etc.

In TCL, we can add comments in three ways .

1. **Complete Line Comments:**

For complete line comments, we need to use # sign in beginning. For example

```tcl

# This line is commented... 
puts "Hello World!"

```

 

**2\. Inline Comments:**

Sometimes we need to write a comment just after finishing our code on the same line. In such cases, we can use inline comments.  Inline comments start with ;# in line. For example :

```tcl

puts $tcl_version ;# This will print TCL Version

```

 

**3\. Block Comments:**

Sometimes we need to add comments to the block of line or to the complete procedure. In such case, we can use block comments. We need to use if with condition 0 for block comments. For example :

```tcl

puts "This line is not commented !"

if 0 {

This is an example of multi-line comments.

This complete block will be considered as comments.

}

puts "Even this is not comment"

```

Try to use these types of comments in TCL scripts !
