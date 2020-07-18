# My Vim Cheatsheet and all you need to know. 
This is meant for people who are new to Vim and I will be updating it along the way.
Feel free to alert me of any errors or additions. 

### Added a test.txt file with 400 lines of lorem ipsum to download/copy for fiddling around with vim commands. 

---
```bash
vim nameOfFileGoesHere  # to open a new file with that name or edit an existing file in the terminal. 
```

## Modes
```bash
# Default mode is Normal/Command mode. 
# Insert mode is for typing into the editor.
# Line mode to do stuff with the file like saving.
ESC           # Normal/Command mode, always returns here. 
i             # Insert Mode
:             # Line Mode
```

## Basics
```bash
:help         # to open help
:o file       # to open file
:saveas file  # to save a file as
:close        # to close current pane
```

## Commands 
``` bash
:wq                 # writequit to save and exit the file.
:w                  # to save but not quit. 
:q!                 # to exit without saving. ( ! specifies forced action, :q will prompt if edited). 
hjkl                # for left bottom top right navigation respectively.
CTRL f/F / PGDOWN   # to move forward one page.
CTRL b/B / PGUP     # to move back one page. 
w                   # to move forward one word including punctuations, will jump to punctuations.
W                   # to move forward one word ignoring punctuations, skips them. 
b                   # to move back one word not including punctuations, will jump to punctuations. 
B                   # to move back one word ignoring punctuations, skips them.
<number> w/W/b/B    # the number specifies how many words you wish to jump. 
0                   # to move to the start of the line including indentation. 

Shift ^             # to move to the start of the word in the line, excluding indentation. 
Shift $             # to move to the end of the line.
G                   # to move to the bottom of the file.
gg                  # to move to top of the file.
<line number> gg    # the number specifies which start of the line to jump to.
:<line number>      # to move to line number only in LINE mode. 
:$                  # to move to the end of file only in LINE mode.
CTRL g/G            # to check total lines in file, current line, percentage to end, current column. 
g CTRL g            # to check extra info, words, total words and bytes.
:set ruler          # to display current line and column on bottom right hand corner.
x / dl              # to delete a letter on the cursor. 
X / dh              # to delete a letter to the left of the cursor. 
dw                  # to delete an entire word from the starting cursor to the next word.  
dl                  # to delete the text on the cursor. 
dj                  # deletes current line and line below you as the motion is supposed to bring you there.
dk                  # deletes current line and line above you. 
d0                  # to delete to the start of line not including current position.
d$                  # to delete to the end of line including current position.  
dd                  # to delete the entire line. 
```

