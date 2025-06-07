    Ctrl+B D — Detach from the current session.
    Ctrl+B % — Split the window into two panes horizontally.
    Ctrl+B " — Split the window into two panes vertically.
    Ctrl+B Arrow Key (Left, Right, Up, Down) — Move between panes.
    Ctrl+B X — Close pane.
    Ctrl+B C — Create a new window.
    Ctrl+B N or P — Move to the next or previous window.
    Ctrl+B 0 (1,2...) — Move to a specific window by number.
    Ctrl+B : — Enter the command line to type commands. Tab completion is available.
    Ctrl+B ? — View all keybindings. Press Q to exit.
    Ctrl+B W — Open a panel to navigate across windows in multiple sessions.






##Start a new named session:

tmux new -s session_name

##🗂️ Managing Sessions
###List all sessions:

tmux ls

###Attach to a session:

tmux attach -t session_name

###Detach from a session:

Inside tmux, press:

Ctrl + b, then d

###Kill a session:

tmux kill-session -t session_name

###Rename a session:

Inside tmux:

Ctrl + b then :
rename-session new_name
