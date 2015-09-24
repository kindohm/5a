#5a

Highly experimental musical live coding editor in the browser.

If you really, really, _really_ want to try this, serve out this
code from a web server, navigate to index.html, and then type
something like this in the editor after the page loads:

```
seq('melody').pat([1,1,2,1,4,1,1]).notes([0,2,0,4,2,7,0,5]);
```

_Select the code you just typed_, then press `Ctrl-Enter`.

Then type:

```
play();
```

_Select this code_, then press `Ctrl-Enter`. You should now hear a sequence
of notes. To stop:

```
stop();
```

Currently, you _must_ select the code you want to eval.

Sequence timing and scheduling is based off of this article:
http://www.html5rocks.com/en/tutorials/audio/scheduling/
