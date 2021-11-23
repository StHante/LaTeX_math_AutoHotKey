# LaTeX_math_AutoHotKey
A small AutoHotKey script that allows converting some LaTeX maths commands to UTF8 symbols anywhere!

## Install
Get a recent UTF8-version of AutoHotKey. Then just start the `latex.ahk` script with AutoHotKey.

## Usage
This script will convert strings of the form `\somecommand` to UTF8 characters that look like the symbol that LaTeX would produce. In order to trigger the conversion, press the tab key. In order to get the symbol ≈, type `\approx` and then hit the tab key. Since there is no such thing as a "math environment", we have to manually tell the script which regular letters to display as italic math symbols, e.g. `\x`+[Tab] will produce 𝑥.
Furthermore, there are some subscript and superscript characters that can be entered like `_i` or `^p` and subsequently pressing the tab key.

Note that there are a lot of commands that I regularly use in my LaTeX files, but which are not standard. New symbols can easily be added.

There are some additional UTF8-Symbols included, which I regularly use. Moreover, there are shortcuts to the typographic quotation marks `„“”` by pressing [AltGr]+[V], [AltGr]+[B] or [AltGr]+[N], respectively. The variants `‚‘’` can be produced by additionally pressing the [Shift] key.

The script can be stopped and started again by pressing [Alt]+[Home].

## Supported characters
For a list of supported characters, please have a look inside the script.

## Caveats
The script starts with a BOM character that tells AutoHotKey that the script uses UTF8 encoding. Do not delete the first (invisible) character, otherwise the script will not work as intended.

## Adding characters
Just edit the script, copy a line and change the command and the UTF8 symbol, which could be copypasted from the web.


