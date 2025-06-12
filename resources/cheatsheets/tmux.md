# 🧠 `tmux` Cheatsheet (`~/.tmux.conf`)

tmux is a terminal multiplexer — it lets you run and manage multiple terminal sessions within a single window. You can:  
- Split your terminal into multiple panes  
- Create and switch between windows  
- Detach from a session and resume it later, even after logging out  
- Script and automate terminal layouts  

It’s especially useful on remote servers and in long-running CLI workflows.


## 🔧 Basics
| Action                    | Key Binding      |
|--------------------------|------------------|
| Prefix key               | `Ctrl+a`         |
| Send literal prefix key  | `Ctrl+a` `a`     |
| Reload config            | `Ctrl+a` `r`     |
| Source default layout    | `Ctrl+a` `P`     |

---

## 🗂️ Window Management
| Action               | Key Binding        |
|---------------------|--------------------|
| New window          | `Ctrl+a` `c`       |
| Close window        | `Ctrl+a` `&`       |
| Next window         | `Ctrl+a` `Ctrl+n`  |
| Previous window     | `Ctrl+a` `Ctrl+b`  |
| Rename window       | `Ctrl+a` `,`       |
| Move window         | `Ctrl+a` `.`       |

---

## 🧱 Pane Management
| Action               | Key Binding               |
|---------------------|---------------------------|
| Horizontal split     | `Ctrl+a` `s` or `Ctrl+s`  |
| Vertical split       | `Ctrl+a` `v` or `Ctrl+v`  |
| Move between panes   | `Ctrl+a` + Arrow keys or `o` |
| Resize pane down     | `Ctrl+a` `J`              |
| Resize pane up       | `Ctrl+a` `K`              |
| Resize pane left     | `Ctrl+a` `H`              |
| Resize pane right    | `Ctrl+a` `L`              |
| Close pane           | `Ctrl+a` `x`              |

---

## 🖱️ Mouse Mode
| Action        | Key Binding |
|---------------|-------------|
| Enable mouse  | `Ctrl+a` `m` |
| Disable mouse | `Ctrl+a` `M` |

---

## 🧠 Extra Useful Commands
```bash
tmux new -s session_name             # Create new session
tmux attach -t session_name         # Attach to session
tmux kill-session -t session_name   # Kill session
tmux ls                             # List sessions
tmux switch -t session_name         # Switch sessions
