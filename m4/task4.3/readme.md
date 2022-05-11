# TASK 4.3

***Part 1:***

**Subtask 1:**

Every process has 5 states:
	- Running or Runnable (R),
    - Uninterruptible Sleep (D),
    - Interruptable Sleep (S),
    - Stopped (T),
    - Zombie (Z)

**Subtask 2:**

pstree -h PID

![alt text](/m4/task4.3/img/4.3.1.2.png "pstree")

**Subtask 3:**

The 'proc fs' is a virtual file system, containing information about running processes.


**Subtask 4:**

lscpu

![alt text](/m4/task4.3/img/4.3.1.4.png "information about processor")

**Subtask 5:**

ps -axo pid,group,command

![alt text](/m4/task4.3/img/4.3.1.5.png "process extended info")

**Subtask 6:**

Kernel processes operates within kernel address space only. User's processes has it own address space.

**Subtask 7:**

![alt text](/m4/task4.3/img/4.3.1.7.png "process list")

In "STAT" we can see the state of every process, and some additional substates:
< high-priority (not nice to other users)
N low-priority (nice to other users)
L has pages locked into memory (for real-time and custom IO)
s is a session leader
l is multi-threaded (using CLONE_THREAD, like NPTL pthreads do)
+ is in the foreground process group 

**Subtask 8:**

![alt text](/m4/task4.3/img/4.3.1.8.png "process of the current user")

**Subtask 9:**

![alt text](/m4/task4.3/img/4.3.1.9.png "help for the ps command")

**Subtask 10:**

The 'top' command displays information about running processes, like it's PID, priority, used virtual memory, percents of the CPU usage, percents of the memory usage, used physical memory, and others.

![alt text](/m4/task4.3/img/4.3.1.10.png "top example")

**Subtask 11:**

![alt text](/m4/task4.3/img/4.3.1.11.png "top example")

**Subtask 12:**

key "k" allows to kill process by PID

![alt text](/m4/task4.3/img/4.3.1.12.1.png "top kill")

key "c" allows to show absolute path of process

![alt text](/m4/task4.3/img/4.3.1.12.2.png "top absolute path")

**Subtask 13:**

key "m" allows to sort processes by memory usage

![alt text](/m4/task4.3/img/4.3.1.13.1.png "top memory")

key "p" allows to sort processes by cpu usage

![alt text](/m4/task4.3/img/4.3.1.13.2.png "top cpu")

key "t" allows to sort processes by taken time

![alt text](/m4/task4.3/img/4.3.1.13.3.png "top time")

**Subtask 14:**

There are 40 main levels of process prioity, from -20(highest) to 19(lowest). Priority can be changed by "renice" command.

![alt text](/m4/task4.3/img/4.3.1.14.png "renice")

**Subtask 15:**

To change process priority using 'top' command, we should press 'r' button, then insert PID and new 'nice' value.

![alt text](/m4/task4.3/img/4.3.1.15.png "renice with top")

**Subtask 16:**

The command 'kill -1 PID' sends the signal to hangs up the process. 
The command 'kill -9 PID' sends the kill signal to the process. 
The command 'kill -15 PID' sends termination signal. 

![alt text](/m4/task4.3/img/4.3.1.16.png "kill")

**Subtask 17:**

The 'jobs' command displays the list of the jobs the current shell is running in the background and in the foreground.
The 'fg' command moves process to the current shell from background.
The 'bg' command is opposite to 'fg'.
The 'nohup' command allows process to keep running after logging out from the shell.

![alt text](/m4/task4.3/img/4.3.1.17.1.png "bg fg for sleep")


***Part 2:***

**Subtask 1:**

ssh dzhura@192.168.188.31 -p 1314

![alt text](/m4/task4.3/img/4.3.2.1.1.png "simple connection")

ssh-keygen -t rsa

![alt text](/m4/task4.3/img/4.3.2.1.2.png "keygen")

ssh-copy-id asu@192.168.188.219

![alt text](/m4/task4.3/img/4.3.2.1.3.png "copy id")

ssh -v asu@192.168.188.219 

![alt text](/m4/task4.3/img/4.3.2.1.4.png "debug")

**Subtask 2:**

ClientAliveInterval 360
ClientAliveCountMax 0
PermitEmptyPasswords no
AllowUsers user1 user2
PermitRootLogin no
Protocol 2

**Subtask 3:**

ssh-keygen -t rsa -b 4096
ssh-keygen -l -f /home/user/.ssh/id_rsa
ssh-keygen -t rsa -b 4096 -C "Andrew to Mail server"

**Subtask 4:**

![alt text](/m4/task4.3/img/4.3.2.4.1.png "debug")
![alt text](/m4/task4.3/img/4.3.2.4.2.png "debug")