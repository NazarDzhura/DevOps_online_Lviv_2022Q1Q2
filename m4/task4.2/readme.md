
**Subtask 1:**

Each line of '/etc/passwd' consist:
- username
- password exists (x mark)
- user ID
- primary group ID, user belongs to
- user info (full name, room number, work phone, home phone)
- user home folder
- user shell

Each line of '/etc/grup' consist:
- group name
- password exists (x mark)
- group ID
- group members

Pseudo user examples: 
- daemon:х:1:1:daemon:/usr/sbin:/usr/sbin/nologin
- bin:х:2:2:bin:/bin:/usr/sbin/nologin
- sys:х:3:3:sys:/dev:/usr/sbin/nologin
- sync:х:4:65534:sync:/bin:/bin/sync

**Subtask 2:**

UID ranges:
0 - root
1-499 - pseudo users
500-more - ordinary users
UID - unique id of every user, mentioned in '/etc/passwd'

**Subtask 3:**

GID - unique id of every group, mentioned in '/etc/group'

**Subtask 4:**

groups user

id user

![alt text](/m4/task4.2/img/4.2.4.png "Subtask 4")

**Subtask 5:**

useradd -g newUserGroup -md /home/newUser newUser

![alt text](/m4/task4.2/img/4.2.5.png "Subtask 5")

**Subtask 6:**

usermod -l newUserName -oldUserName

![alt text](/m4/task4.2/img/4.2.6.png "Subtask 6")

**Subtask 7:**

/etc/skel is a folder which consist files and directories needed for creation new user's home directory. It contains ".config", ".bashrc", probably ".mozilla", and other files.

![alt text](/m4/task4.2/img/4.2.7.png "Subtask 7")

**Subtask 8:** 

deluser --remove-home newUser
deluser --remove-all-files newUser

![alt text](/m4/task4.2/img/4.2.8.png "Subtask 8")

**Subtask 9:** 

usermod -L newUser
usermod -s /sbin/nologin newUser
passwd -l newUser

![alt text](/m4/task4.2/img/4.2.9.png "Subtask 9")

**Subtask 10:**

passwd -d newUser

![alt text](/m4/task4.2/img/4.2.10.png "Subtask 10")

**Subtask 12:**

User can ususally read, write or an execute a file. Access right for each action is marked as 'r', 'w' 'x', collected in 'rwx' group. Access rights are separated for user, for his group, and for the others. It looks like 'rwxrwxr--' for each file.

**Subtask 13:**

User can ususally read, write or an execute a file. 

**Subtask 14:**

chown new-owner  filename
chmod u=rw,ug+rw,o=r permissions.txt

![alt text](/m4/task4.2/img/4.2.14.png "Subtask 14")

**Subtask 15:**

octal representation is 'r'=4, 'w'=2, 'x'=1. Summary 'rwx'=7, 'rx'=5. Command 'umask' sets default access rights for newly created files.

**Subtask 16:**

Sticky bit restricts user to remove files from directory, if he is not file owner.
chmod 1775 *file*
ls -ld
ls -ld /tmp

![alt text](/m4/task4.2/img/4.2.14.png "Subtask 14")