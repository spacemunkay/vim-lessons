# 05_deleting_text

## NOTE: In case of emergency, just hit ESC and type :q!

There are a number of ways to delete text within vim.  While in 'insert' mode, you can use the backspace and delete keys.

While in 'normal' mode you can use:

* x
* d

You might make some mistakes, so use 'u' to undo changes, and ctrl + r to redo.

# Highlight a character in this line and use the 'x' command while in 'normal' mode to delete it.

# Type 'u' to undo that last change you did.

The 'd' command requires another command to be combined with it in order for it to function. Some common combos:

* dw
* dd
* de
* db
* d$
* dj

# Highlight a character at the beginning of a word in this line and type the dw command while in 'normal' mode to delete an entire word.

# Put the cursor on this line and type the dd command to delete the entire line.

# Save the file, then type the following to start the next lesson: :e 06_copying_and_pasting_text.md
