# linux-macos-unix
Linux, MaxOS, and other Unix-derivative operating systems, kernels, window managers, programs, shells, commands, and configuration

# vi (and vim)

| ESCAPE commands  | (press ESC key to enter escape/command mode)             |
| :------------ | :------------|
| i | enter insert mode, at cursor (type away) |
| a | enter append/insert mode, immediately to the right of cursor (even at end of line) |
| R | overwrite mode, at cursor [note capitalization]|
| x | delete a singe character the cursor is on |
| dd | delete (cut) the entire line the cursor is on |
| 10dd | delete (cut) 10 lines (this one and 9 below) |
| yy | yank (copy) this full line |
| 3yy | yank (copy) three lines, this one and next two) |
| p | paste the most recently yanked/cut or deleted character or line(s) (immediately after this one) |
| u | undo last command (repeat to undo previous commands) |
| J | join this line and the next, with a space in between [note capitalization]|
| ^ | go to beginning of line the cursor is on |
| $ | go to end of line the cursor is on |
| ZZ | write file or save changes, and exit [note capitalization]|

| Other commands | (generally must hit ENTER/RETURN key after each command) | 
| :------------ | :------------|
| /hello | search forward to find the next instance of word "hello" in text |
| / | repeat the last find |
| ?hello | search backward to find the previous instance of word "hello" in text |
| :q! | do NOT write file or save changes, just exit |
| :w | write changes to this file |
| :w file2 | copy the current state of this file to new file named file2, and start editing that file |
| :wq | write changes to file and quit (exit) |
| :$ | go to the last line of file |
| :1 | go to the first line of file |
| :218 | go to line number 218, if there is one (or to last line of file if shorter than 218 lines) |
| :set nu | turn on line numbers (use :set nu! to toggle line numbers back off) 
| :%s/delete/del/g | substitute/replace "delete" with "del", globally (entire file) |
| :%s/,//g | substitute/replace all commas, globally (careful! remember, :w to save first, u for undo, :q! to "bail out") |
| :%s/\$//g | globally remove (replace with nothing) all dollar signs ($) |
| :!ls | run a shell command (ls, in this case), then return to editing this file |
| :UP ARROW | navigate UP (or DOWN) through previous commands used in this mode [note ENTER/RETURN not needed] |
