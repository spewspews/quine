Quine.c is my first self-reproducing program. Nothing fancy.
About the least inventive quine you can write.

Even though it is bigger, I actually prefer insquine.c a little more
because it inserts itself at the @ symbol.

Rotquinegen.c is a program that generates the
file rotquine.c. Rotquine.c is a quine that stores its
representation of itself shifted out of the ascii range
so that you are not able to run strings against it to
easily check if there is embedded source code in the
executable. This makes Ken Thompson's trusting trust
attack harder to detect. If a cryptographic cipher were
used the attack would be practically impossible to detect.

I then adapted insquine.c to insrotquinegen.c which generates
insrotquine.c. This quine removes the only remaining ascii
string (`"0 };"` that can be found in rotquine.c)
that could possibly indicate that the executable is a quine.
