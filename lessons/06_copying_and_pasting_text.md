# 06_copying_and_pasting_text.md

## NOTE: In case of emergency, just hit ESC and type :q!

In vim, deleting text is essentially always 'cutting' text. So, now that you know how to delete/cut text, you should learn how to paste.

You can use these commands to paste text:
* p
* P

# Put your cursor on this line and delete this line with dd then paste it back with p

What if you don't want to delete a line of text to copy it? You can use the yy command to copy an entire line.

# Put your cursor on this line and copy it with yy then paste it with p

What if you only want to copy part of some text, and not the entire line? Well, first, you need to learn to use 'visual' mode to first highlight text.

# Put your cursor on this line and type v to enter 'visual' mode.  Use h and l to move the cursor to highlight text. Hit ESC two times to return to 'normal' mode.

Got the hang of it?  Now, after you highlight text you can copy it by pressing y

# Put your cursor on this line and type v to enter 'visual' mode.  Use h and l to move the cursor to highlight text. Once some text is highlighted, press y and then paste it with p

Like the d command, you can combo the y command to avoid entering the visual mode:

* yw
* yb
* yy
* y0
* y$

# Put your cursor at the beginning of a word on this line and type yw and then p.

# Save the file, then type the following to start the next lesson: :e 07_something.md
