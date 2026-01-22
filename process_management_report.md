
# Task 5 - Process Management Report (Linux)

## Objective
To learn process monitoring, killing processes, and managing services using Linux CLI.


## 1) List Running Processes

### Command Used
- ps
- ps -ef
- ps -ef | grep <process>

### Output Summary
- Listed all running processes with PID, user, and command details.
- Used grep to find a specific process quickly.


## 2) Monitor Live Processes using top

### Command Used

top


### Output Summary

* Monitored processes in real time and checked CPU/RAM usage.
* Identified the highest resource-consuming processes.

## 3) Check Process States

### Command Used


ps -eo pid,ppid,user,stat,%cpu,%mem,cmd --sort=-%cpu | head -10


### Output Summary

* Displayed top CPU processes with PID and state information.
* Understood process states like R, S, T, and Z.


## 4) Create and Kill a Process

### Command Used


sleep 300 &
ps -ef | grep sleep
kill <PID>
kill -9 <PID>


### Output Summary

* Created a dummy process and found its PID using ps.
* Terminated the process using normal kill and force kill.


## 5) Service Management using systemctl

### Command Used


systemctl status ssh
sudo systemctl start ssh
sudo systemctl stop ssh
sudo systemctl restart ssh
sudo systemctl enable ssh
systemctl is-enabled ssh

### Output Summary

* Managed services by checking status and using start/stop/restart commands.
* Enabled service at boot and verified it using is-enabled.


## 6) System Resource Monitoring

### Command Used

free -h
df -h
uptime

### Output Summary

* Checked memory and disk usage using free and df commands.
* Verified uptime and system load average using uptime.


## Final Conclusion

This task improved my understanding of Linux process monitoring and control.
I can now manage processes, services, and system resources effectively.


