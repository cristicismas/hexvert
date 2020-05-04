# HEXVERT

### Hi!

This is a little python script that converts a hex string into a normal string (utf-8), little edian or big edian bytes!

I've made this to help me a bit in my reverse-engineering CTFs, but if anyone wants to improve this, you are free to make your pull request and I'll look over it.

### Usage

The script accepts 2 arguments:

The *first* argument is a hex string (prepended by 0x). Example: 0xdeadbeef

The *second* argument is the thing you want to convert to. This can be one of the following:

1. _little_ - Convert to little edian.
2. _big_ - Convert to big edian.
3. _string_ - Convert to an utf-8 string (if possible)

