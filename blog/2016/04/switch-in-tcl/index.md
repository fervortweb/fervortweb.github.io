---
title: "Switch in TCL"
date: "2016-04-04"
categories: 
  - "tcl"
---

Like other programming languages, TCL also provides support to switch case. It is used to test multiple conditions. In TCL switch, we don't need to write break statement like other languages. To achieve switch case functionality we can also use if else statements .

Let us see syntax of switch case :

switch option **switch\_expression** **switch\_expression\_1**  { body\_1 } **switch\_expression\_2** { body\_2 } **switch\_expression\_3** { body\_3 } **default** { default\_body }

**switch\_expression** can be a number, alphabet or string . If **switch\_expression** match with any subsequent **switch\_expressions** then body corresponding to that expression will be executed. **default** block will be executed if **switch\_expression** doesn't match with any subsequent expressions.

options can be :

\-exact : Use exact matching (default)

\-glob : When matching string to the patterns like \*, ? (i.e. the same as implemented by the string match )

\-regexp : When matching string to the patterns, use regular expression.

**Let us see some examples :** _1\. switch case with numbers_ :

```tcl

#!/usr/bin/tclsh set number 5; switch $number 1 { puts "One" }

2 { puts "Two" }

3 { puts "Three" }

default { puts "Invalid Number." } } 

```

Output : $tclsh main.tcl Invalid Number.

 

2\. Switch case with string :

```tcl #!/usr/bin/tclsh set country\_code "US"; switch $country\_code { US { puts "United States of America" } IN { puts "India" } UK { puts "United Kingdom" } default { puts "Invalid Country Code" } } ```

 Output: $tclsh main.tcl United States of America

 

3\. Switch using option:

```tcl
#!/usr/bin/tclsh set var\_string computer;

switch -glob $var\_string { com\*er { puts "Matched with com\*er" } default { puts "Invalid !" } } 

```tcl

Output: $tclsh main.tcl Matched with com\*er
