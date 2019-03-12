+++
title = "bcrypt.net Core"
date = 2018-12-23T00:00:00

# List format.
#   0 = Simple
#   1 = Detailed
#   2 = Stream
list_format = 2

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = ""
+++


At the release of .net core 1.0, there was no way to trivially use bcrypt password hashing. A .net library existed, but it had been abandoned by the author.

I took it upon myself to port this library to .net core. I have been maintaining it ever since and it is currently the most popular bcrypt library for .net core!