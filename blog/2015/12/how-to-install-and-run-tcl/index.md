---
title: "How to install and Run TCL"
date: "2015-12-30"
categories: 
  - "tcl"
---

In this article, we will see how to install TCL on windows and run it. First we will download TCL from this link [http://www.activestate.com/activetcl/downloads](http://www.activestate.com/activetcl/downloads)  .

Choose the binaries depend on your System types either 64 bit or 32 bit. Double click on downloaded setup to start installing TCL.

![installing-tcl](images/installing-tcl-1.png "installing tcl")

Accept license agreement.

![TCL license agreement](images/installing-tcl-1.png "TCL license agreement")Choose path. I am installing on C:\\Tcl default path

![installing tcl path](images/installing-tcl-path-1.png "installing tcl path")

So TCL is installed on your windows.  Now we will set path of C:\\Tcl\\bin\\ directory so, we can run it from any location.

To set path just copy the path up to bin directory ( In my case it is C:Tcl\\bin\\ ) and fire command like this

![set tcl path windows](images/set-tcl-path-windows-1.png "set tcl path windows")

Path is set so we can run TCL from any location. Lets try to run it from D drive. First create one small TCL and save it on D drive with name Hello.tcl . So the path is D:\\Hello.tcl

![tcl in notepad](images/tcl-in-notepad-1.png "tcl in notepad")

To run this file open command prompt and go to path D: and execute command **tclsh Hello.tcl** like this .

![running tcl](images/running-tcl-1.png "running tcl")

It will print output **Hello World !**
