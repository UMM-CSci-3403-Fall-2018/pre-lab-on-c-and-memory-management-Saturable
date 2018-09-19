# Leak report

There is a leak of 46 bytes in 6 blocks.
These are at the following locations:
- 0x4C31B25
- 0x10882E
- 0x10889A
- 0x108946

This can be fixed by freeing the space of the cleaned string, but only if it has more than 0 characters.
Otherwise, a whitespace string could throw errors. 
