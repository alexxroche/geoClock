geoClock
========

Terrestial sunlight clock - based on an example from bl.ocks.org/mbostock [0]
using <a href="d3js.org">d3js.org</a>

bl.ocks.org/mbostock/9658291,
bl.ocks.org/mbostock/4597883,
bl.ocks.org/mbostock/9232962,
bl.ocks.org/mbostock/4597134 and other great code examples.


Somewhere in my youth I saw a GeoChron; a type of fancy wall clock that impressed me.
I suspected that it was for those with more disposable income than taste and wealth immigrants
that felt a need to impress. Today you can create one using an old laptop, this code and a spare
screen.

After xkcd.com/1335 inspired Mr Bostock, this code was created to add, "the closest thing to NTP
within javascript" combined with a geoClock. The problem is that NTP, (Network Time Protocol) is clever, complicated, and not something that javascript should be messing with, (when the gods gave us C.) <a href="http://time.is/">time.is</a> is the closest that I know of to NTP on the web, other than time-stamped error messages... so why not create code that tries a few things and estimates which is best.

Basicly, start with DateTime() and see if any noise out on the web can be used to suggest improvements, accuracy and location.
