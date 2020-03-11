falseknees-atom
===============

A simple Lua script that generates an Atom Feed of the fantastic
[False Knees][falseknees] webcomic.

Requirements
------------

You need to have [Lua][lua] (5.3 or later) and [LuaSocket][luasocket] installed.

Usage
-----

Executing `falseknees-atom.lua` will write an Atom Feed with all the comic
strips to stdout. When you are using a feed reader that can take it's input from
an external binary, you can just point it to the script. E.g. here is an entry
for [Newsboat][newsboat]'s `~/.newsboat/urls` that I use:

    exec:~/src/falseknees-atom/falseknees-atom.lua

`~/src/falseknees-atom/` is where this repo lives on my machine. Adapt the path
to fit wherever you put it.

Why?
----

I want to know when the latest comic arrives, but
<http://falseknees.com/rss.xml> does not seem to get updated any more :(.


[falseknees]: https://falseknees.com
[lua]: https://lua.org
[luasocket]: http://w3.impa.br/~diego/software/luasocket/home.html
[newsboat]: https://newsboat.org/
