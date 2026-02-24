## uEmacs/PK/ER 4.0.16

First, enjoy this anti-advocacy I found in 4.0.15, , from whom I can
only guess: 

----
    Very old, very crusty, full screen editor based on MicroEMACS 3.9e. 

    Please don't use this, the whole thing only exists and is (badly)
    maintained because I have been using this thing for decades, and my
    fingers cannot be retrained from the strange keybindings this old
    version of uemacs uses. 

    Despite the name, the keybindings bear only passing resemblance to real
    emacs, and the choices also tend to be incompatible with other editors
    even when those editors keybindings are configurable.

    This is a *bad* editor.  Really.  Unless you have used it since the
    1980s, and have untrainable fingers, you should absolutely walk away and
    never look back.  I've updated it minimally over the years to keep it
    kind of working, but only kind of.

    So this is a simplistic editor, written for an age when you had 64kB
    limits and 300 or 1200 baud terminals were common.  It was not a better
    age, and this is not a better editor. 
----

Not a better age perhaps, but a more innocent; the internet had not been
conceived, there were no social media, and hackers were not predatory
sociopaths, but generous introverts who labored tirelessly simply to
advance the art of coding.  

So, a little history of MicroEmacs:

Daniel Lawrence and David Conroy apparently had a fondness for the
'real' emacs of the early 80's, which would eventually become 'Gnu
Emacs'.  An editor that would let you move freely around a crt screen
and just type what you were thinking was novel then; most code was typed
or punched a line at a time, slowly and painfully, and emacs addressed
that pain.  And it was touted by Richard Stallman, a ferocious partisan of
open source, free-as-in-speech-not-free-as-in-beer software. 

But even in 1985, gnu emacs was a bloated monster with ambitions of
owning your desktop.  It was hard to install and harder to learn, a
resource hog fit only for the nerdiest of believers.  It got worse over
time.  (All this, IMHO.)

MicroEmacs was the anti-emacs: small, light, fast, accessible, freely
installable on even the puniest machines:  CPM, Atari, Amiga, DOS, RSX,
RSTS, Mac, 3 flavors of Unix.  But you could only find it if you knew it
was there. 

I got version 3.8g from a DECUS resource tape in 1988, fiddled with it
until it compiled, and fell in love.  I had my own private fork, which I
hacked mercilessly and shared with one or two colleagues.  I wrote all
my code with it for 30 years, porting it to Win-NT, VAX/VMS, Alpha/VMS,
and finally Linux.  Eventually, architecture changes and software
upgrades outran my skills, and stuff started breaking.  The macro
language became unusable. 

I read somewhere that Linus Torvalds' favorite editor was MicroEmacs. 
Surely, if Linus uses it (not 'used' it), it's still maintained.  Of
course, Github. 

I guess Linus (not yet Dr Torvalds) was in the market for a neat litte
editor at about the same time I was, and somehow got wind of MicroEmacs,
about version 3.9e.  He didn't do all the work on it himself; Dr Petri
Kutvonen, a computer science professor at the University of Helsinki,
did most of the mods that made it useful, from about 1991 onwards.  His
last update, which he dubbed 4.0.15, was zipped in 1996.  It builds on
Ubuntu with barely an edit, after 30 years!  That's stable. 

But what happened after 1996?  Is Linus Torvalds still using it? 

He has his own fork, with extremely sketchy change logs, updated LAST
MONTH.  Lean it is:  he took out many features, some of which I depend
upon, and stripped most of the conditional code intended to make it
portable.  Now, I get dumping Amiga support, but Windoze needs a good
editor, and a few diehards still use VMS.  Oh, well.  I'm sure he has
his reasons.  Maybe he doesn't do windows (or use multiple windows). 

In any case, I thank him for the work he and Dr Kutvonen put into it,
and for keeping the flame alive.  Oh yeah, and for giving away the
kernel that runs about half the computing machines on Earth.  That's not
hacking, that's Prometheus. 

So this is 'my' version of MicroEmacs, derived from Dr Kutvonen's
uEmacs/PK 4.0.15.  I hacked it enough that I thought it good to give it
a 'minor-version' upgrade number, 4.0.16, after Dr Kutvonen's 4.0.15. 
The significant changes: 

    - automatic pre-edit backup, when autosave is turned on.
    - expanded keyboard support for Gnome (and probably VT220).
    - horizontal (jump) scrolling of wide files.
    - a 'list-internals' function.

And probably a bunch of insidious bugs that would embarass a real
computer scientist, which I am not. 

Try it if you like typewriters and yo-yos and knives that rust.

    - Earl Roosa (earlroosa@gmail.com)  20260211_07_16:10:42
