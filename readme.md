# jquery-style-guide-javascript-aptana

Aptana JavaScript Code Formatter profile based on [jQuery JavaScript Style
Guide](http://docs.jquery.com/JQuery_Core_Style_Guidelines).

## Installation

1. open Aptana IDE
2. open the Preferences window
3. drill down: Atpanta -> formater
4. click Import and select the provided XML file
5. done!

## Known Issues

### Functions with no arguments

When Functions do not have any arguments they get formated like `func( )`.

There doesn't seem to be an Aptana setting to say if this function dosen't
have any arguments then don't add the spacing.  The same problem show the
function declarations too: `function func( )`.  Anonymous functions with no
arguments look well with no space between the parentheses: `function()`.

### Function calls with an object literal at the beginning or end

No space should be on either side of the argument:

    foo({ a: "alpha", b: "beta" });

It appears that the intention is to avoid spaces between braces and
parentheses, maybe brackets too, when they just sit next to each other.
There doesn't seem to be a setting for this special case and because
the spaces are turned on after the opening and before the closing
parenthesis/brace/bracket, they will occur between them too.
