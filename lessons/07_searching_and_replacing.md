# 07_searching_and_replacing.md

## NOTE: In case of emergency, just hit ESC and type :q!

There are a number of ways search within VIM.  One handy way is to use * and # to jump to a word that matches the word underneath the cursor.  Once you have matches you can type n or N to jump to next or previous matches.

# Put your cursor over the word 'word' and press * or # a few times.

Another way to search is to use / or ? and then type the word you're looking for, then hit enter.

# Type /word and hit enter.  Then hit n or N a few times to jump between matches. Then try ?word

So, how do you search and replace?  This part is not so intuitive.  You must use the substitute commands which looks like:

:%s/searchterm/replaceterm/gc

There's a lot going on with this command, here's the breakdown:

* : - enter command mode
* % - this tells the command to affect the entire document.  Leave it out to only affect the current line.
* s - use the 'substitute' command
* searchterm - this is where you type the term you're searching
* replaceterm - this is the text that will replace your search term
* g - global
* c - this prompts for a yes/no confirmation before replacing terms. Leave it out to replace everything instantly.

# Type :%s/word/thing/gc and hit enter.

There are a few caveats with using :s.  The following characters must be escaped with a \ in order to search for them.

. * \ [ ^ $

If you want to include a space in your search term, you must type \s or a \ with trailing space.

# Type :%s/\^\s\$/caret\ dollar\ sign/gc

# Save the file, then type the following to start the next lesson: :e 08_formatting.md
