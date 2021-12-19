# LineBrowser — Fast and Simple lightweight Browsing

LineBrowser is a Fast and Simple lightweight Browser designed 
to target linux systems. Especially single-board computing systems such as
the Raspberry Pi. This browser is written in python using PyQt5.

## Code notes

### Tabbing

Adding tab support complicates the internals of the browser a bit, since we
now need to keep track of the currently active browser view, both to update
UI elements (URL bar, HTTPs icon) to changing state in the currently active
window, and to ensure the UI events are dispatched to the correct web view.

This is achieved by using intermediate slots which filter events, and by
adding signal redirection (using lamba functions to keep it short).

### To do
- Currently nothing

Request for things in the issues tab!

## Other licenses

Icons used are created by [Yusuke Kamiyaman](http://p.yusukekamiyamane.com/).
