# Notes for some command tools
## tmux
This note is based on [this blog](https://www.cnblogs.com/wangqiguo/p/8905081.html)
#### session
* `tmux new -s session_name`: create a new session(cmd in shell)
* `ctrl+b d`: **detach** session, return to shell
* `tmux ls`: session list(cmd in shell)
* `ctrl+b s`: session list
* `tmux a -t session_name`: Attach to a new session, enter a session(cmd in shell)
* `tmux switch -t [name]`: Switch to a session
* `tmux detach OR ctrl - b - d`: Detach from a session
* `tmux kill-session -t session_name`: kill a session(cmd in shell)
* `ctrl+b :` and `kill-session -t session_name`: kill session
* `tmux rename -t old new`: rename a session(cmd in shell)
* `ctrl+b $`: rename a session
 
#### window
* `ctrl+b c`: **create** a window
* `ctrl+b p`: **previous**  window
* `ctrl+b n`: **next** window
* `ctrl+b w`: list all window
* `ctrl+b l`: neighbor window
* `ctrl+b 2`: switch to 2rd window
* `ctrl+b &`: close window

#### pane
* `ctrl+b %`: vertical split
* `ctrl+b "`: horizontal split
* `ctrl+b o`: one by one
* `ctrl+b up,down,left,right`: arrow switch
* `ctrl+b <space>`: rearrangement of all panes
* `ctrl+b z`: maximum current pane, restore after double cmds
* `ctrl+b x`: exit current pane

#### shadowsocks
* vim /etc/shadowsocks.json
* ssserver -c /etc/shadowsocks.json -d start 
