# top-cheat-sheet
# Top Command Cheat Sheet

`top` is a command-line task manager that displays system processes and other performance metrics.

---

## Key Sections in `top`

- **Top bar**: System summary including uptime, CPU, memory usage, load average, etc.
- **Task list**: Shows running processes with details like PID, user, CPU%, MEM%, and command name.

---

## Key Commands Inside `top`

| Key   | Action                                                         |
|-------|-----------------------------------------------------------------|
| `h`   | Help: Show detailed help on commands.                          |
| `q`   | Quit: Close `top`.                                             |
| `Space`| Refresh: Refresh the process data immediately.                |
| `k`   | Kill: Prompt to kill a process (enter PID).                    |
| `r`   | Renice: Change priority of a process (enter PID and priority). |
| `P`   | Sort by CPU usage (default).                                   |
| `M`   | Sort by memory usage.                                          |
| `N`   | Sort by process ID (PID).                                      |
| `T`   | Sort by cumulative CPU time.                                   |
| `u`   | Filter by user: Enter username to display their processes.     |
| `l`   | Toggle display of load average and uptime.                     |
| `t`   | Toggle display of task and CPU status.                         |
| `m`   | Toggle memory usage details.                                   |
| `c`   | Toggle full command path.                                      |
| `W`   | Write configuration to save user settings.                     |

---

## Additional Notes

- Pressing the **number keys** (like `1`) displays individual CPU core usage.
- To increase or decrease the refresh rate (`delay`), press `d` and enter a value in seconds.
- For interactive process killing or renicing with fewer parameters, `k` and `r` are your go-to shortcuts.

---

## Usage Example

```bash
top -u username  # Show only processes for a specific user
top -p 12345     # Monitor a specific process by its PID
top -d 5         # Set refresh interval to 5 seconds
```

---

## Related Commands

- `htop`: A more user-friendly interactive process viewer.
- `ps`: For listing processes in a scriptable format.

---
