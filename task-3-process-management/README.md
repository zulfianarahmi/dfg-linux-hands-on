# 3. Process Management

For detailed explanations, check out my [Medium post on Task 3](https://medium.com/@zulfianarahmi4/dfg-linux-hands-on-homework-task-3-6f4bd5b2205c)

## Task 3.1: Start a long-running process using the command `sleep 500 &` and note its PID.

```bash
sleep 500 &
```

## Task 3.2: Run `stress` in a separate terminal tab to simulate light CPU and memory usage:

```bash
stress --cpu 1 --vm 1 --vm-bytes 512M --timeout 30s
```

## Task 3.3: Use `top` or `htop` to monitor the system and identify resource usage by processes.

```bash
top
# or
htop
```

## Task 3.4: Use `ps` to verify the `sleep` process is running.

```bash
ps aux | grep sleep
```

## Task 3.5: Use `df` and `du` to check disk space usage, particularly focusing on large files in the system.

```bash
df -h
```

## Task 3.6: Use `free` to monitor memory usage while `stress` is running.

```bash
free -h
```

## Task 3.7: Use `ps -aux` and `awk` to log processes consuming more than 10% CPU into a file `high_cpu.log` every 5 seconds.

```bash
while true; do ps -aux | awk '$3 > 10 {print $0}' >> high_cpu.log; sleep 5; done
```

## Task 3.8: Kill the long-running process started in Task 3.1 using its PID.

```bash
kill <PID_of_sleep>
```

or

```bash
killall sleep
```

---

## Challenges:

- Understanding basic process concepts, like foreground and background.
- Identifying a specific process among many others in the system.
- Interpreting the output of commands like ps, top, or htop.
- Managing system resources with tools like stress, and understanding its impact on CPU, memory, and disk.

## Learning:

- Using & to run processes in the background while keeping the terminal active.
- Using ps aux | grep to filter out specific processes.
- Understanding data from monitoring tools (like top, htop) to keep an eye on system resources.
- Practicing resource management with commands like stress and monitoring its effects with free, df, or du.
- Controlling processes using PID, such as killing processes with kill.
