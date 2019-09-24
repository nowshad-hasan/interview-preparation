## Contents

* [Linux](#linux)
* [Windows](#windows)
* [Read More](#read-more)

### Linux

* <b>Name and describe a different Linux/Unix command for each letter of the alphabet. But also, describe how a common flush toilet works.</b></br>

  “The first question helps illustrate the breadth of their CLI chops. But just as important is describing how a toilet works; it demonstrates their well-roundedness and/or ability to think, reason, and hypothesize on their feet.” – Michael Jennings, Computer Systems Engineer, Linux Server/Cluster Admin, Lawrence Berkeley National Laboratory.

* <b>What open source projects are you interested in?</b></br>

  “A really good candidate, even if they’re junior will have found the project they’re interested in and be committing a bit back or writing some documentation. They will be really plugged into what the open source community is doing. They’ll have run Apache Zookeeper, for example. They’ll have wrestled with the code and looked through the docs and actually understand how this works. And maybe they haven’t run it in production but they understand at a high level how the pieces interact, how you can take advantage of it, and what the benefits are.” – Joe Smith, Twitter.

* <b>I have this server which seems to drop off the local net every so often, and comes back on its own. How would you debug this?</b></br>

  “I give them problems that I hope they don’t already know to see how they work through them. I have a list of troubleshooting questions and guesstimate which one to use depending on the level of the candidate.” – Marc Merlin, Senior Linux Server Admin, Google.

* <b>How does TLS work?</b></br>

  “It helps me understand how good they are with security topics. How in-depth they go with their answer – how comfortable they are – tells me a lot.” – Konstantin Ryabitsev, Director of Collaborative IT Services at The Linux Foundation.

* <b>What do you know about SUSE, why do you want to work here, and what’s the role of open source in the market?</b></br>

  “Candidates can show their motivation through concrete contributions or visibility in an open source community and an understanding of what companies do. They will have researched SUSE before they come and talk to us. The bare minimum is that they have installed openSUSE and actually played around with that.” – Marie Louise van Deutekom, SUSE’s Global Human Resources Director.

* <b>What about this job appeals to you?</b></br>

  “That’ll tell me how much they’ve thought about it. A.) You need to make sure you understand your strong points – know yourself. B.) Know what the job entails. And C.) make sure that when you speak you do it sincerely and honestly and be yourself. Probably the biggest mistake that people make is trying to put on a facade.” – Steve Westmoreland, Chief Information Officer, The Linux Foundation.

* <b>Tell me a “war story” about a situation that went wrong and what you did to help on your own initiative.</b></br>

  “In an interview I don’t dive into “tech” skills. Coding languages and various packages can be learned. I am firmly of the belief that you learn a heck of a lot more about a candidate in an interview by asking him or her to tell you “war stories.” If they stumble on that, then you’re looking at a Drone. (Next!)” – Tim Hoogasian, Solutions Project Manager at Newstar Digital and former Technical Project Manager at Dell.

* <b>Print the content of a file backwards.</b></br>

  “I like broad questions where each person could give a different answer depending on their depth of knowledge. My personal answer is 8 characters not including the filename.” – Marc Merlin, Google.

* <b>Nothing in particular.</b></br>

  “I don’t have one question that everyone needs to know. If someone doesn’t know the answer to something, that’s great. We’ll work through the problem and come to the answer together.” – Joe Smith, Twitter.

* <b>Let’s say you maintains a backup on regular basis for the company you are working. The backups are maintained in Compressed file format. You need to examine a log, two months old. What would you suggest without decompressing the compressed file?</b></br>

  To check the contents of a compressed file without the need of decompressing it, we need to use ‘zcat’. The zcat utility makes it possible to view the contents of a compressed file.

  `# zcat ­f phpshell­2.4.tar.gz`

* <b>You need to track events on your system. What will you do?</b></br>

  For tracking the events on the system, we need a daemon called syslogd. The syslogd daemon is useful in tracking the information of system and then saving it to specified log files.

  Running ‘syslogd‘ application in terminal generates log file at the location ‘/var/log/syslog‘. The syslogd application is very useful in troubleshooting Linux sytems. A sample log file looks similar to below.

  ![System Log](/image%20assets/system_log.jpeg)</br>

* <b>How will you restrict IP so that the restricted IP’s may not use the FTP Server?</b></br>

  We can block suspicious IP by integrating tcp_wrapper. We need to enable the parameter “tcp_wrapper=YES” in the configuration file at ‘/etc/vsftpd.conf’. And then add the suspicious IP in the ‘host.deny’ file at location ‘/etc/host.deny’.

  **Block IP Address**</br>
  Open ‘/etc/hosts.deny’ file.</br>
  `# vi /etc/hosts.deny` </br>
  Add the IP address that you want to block at the bottom of the file.

* <b>Tell us the difference between Telnet and SSH?</b></br>

  Telnet and SSH both are communication protocol which are used to manage remote system. SSH is Secured, which requires exchanging of key opposite of telnet which transmit data in plain text, which means telnet is less secure than SSH.

* <b>You need to stop your X server. When you tries to kill your X server, You got an error message that you cannot quit X server. What will you do?</b></br>

  When killing a X server, it won’t work normal way like doing ‘/etc/init.d/gdm stop’. We need to execute a special key combination ‘Ctrl+ Alt+ Back Space’ which will force X server to restart.

* <b>What is the difference between command ‘ping’ and ‘ping6’?</b></br>

  Both the commands are same and used for the same purpose except that the fact that ping6 is used with ipv6 IP address.

* <b>You want to search for all the \*.tar files in your Home directory and wants to delete all at once. How will you do it?</b></br>

  We need to use find command with rm command to delete all “.tar” files.</br>
  `# find /home/ ­name '*.tar' | xargs rm ­rf`

* <b>What is the difference between locate and slocate command?</b></br>

   The slocate looks for the files that user have access whereas locate will search for the file with updated result.

* <b>You need to search for the string “Tecmint” in all the “.txt” files in the current directory. How will you do it?</b></br>

  We need to run the fine command to search for the text “Tecmint” in the current directory, recursively.</br>
  `# find -­name “*.txt” | xargs grep “Tecmint”`

* <b>You want to send a message to all connected users as “Server is going down for maintenance”, what will you do?</b></br>

  This can be achieved using the wall command. The wall command sends a message to all connected users on the sever.</br>
  `# echo please save your work, immediately. The server is going down for Maintenance at 12:30 Pm, sharply. | wall`

  ![System Log](/image%20assets/system_down.jpeg)</br>

* <b>What is the core of Linux Operating System?</b></br>

  * Shell
  * Kernel
  * Command
  * Script
  * Terminal

  Kernel is the core of Linux Operating System. Shell is a command Line Interpreter, Command is user Instruction to Computer, Script is collection of commands stored in a file and Terminal is a command Line Interface

* <b>What Linus Torvalds Created?</b></br>

  * Fedora
  * Slackware
  * Debian
  * Gentoo
  * Linux

  Linus Torvalds created Linux, which is the kernel (heart) of all of the above Operating System and all other Linux Operating System.

* <b>Torvalds, Wrote most of the Linux Kernel in C++ programming Language, do you agree?</b></br>

  No! Linux Kernel contains 12,020,528 Lines of codes out of which 2,151,595 Lines are comments. So remaining 9,868,933 lines are codes and out of 9,868,933 Lines of codes 7,896,318 are written in C Programming Language.

  The remaining Lines of code 1,972,615 is written in C++, Assembly, Perl, Shell Script, Python, Bash Script, HTML, awk, yacc, lex, sed, etc.

  **Note** : The Number of Lines of codes varies on daily basis and an average of more than 3,509 lines are being added to Kernel.


* <b>Linux initially was developed for intel X86 architecture but has been ported to other hardware platform than any other Operating System. Do you agree?</b></br>

  Yes, I do agree. Linux was written for x86 machine, and has been ported to all kind of platform. Today’s more than 90% of supercomputers are using Linux. Linux made a very promising future in mobile phone, Tablets. In-fact we are surrounded by Linux in remote controls, space science, Research, Web, Desktop Computing. The list is endless.

* <b>Is it legal to edit Linux Kernel?</b></br>

  Yes, Kernel is released under General Public Licence (GPL), and anyone can edit Linux Kernel to the extent permitted under GPL. Linux Kernel comes under the category of Free and Open Source Software (FOSS).

* <b>What is the basic difference between UNIX and Linux Operating System.</b></br>

  Linux Operating System is Free and Open Source Software, the kernel of which is created by Linus Torvalds and community. Well you can not say UNIX Operating System doesn’t comes under the category of Free and Open Source Software, BSD, is a variant of UNIX which comes under the category of FOSS. Moreover Big companies like Apple, IBM, Oracle, HP, etc. are contributing to UNIX Kernel.

* <b>Choose the odd one out</b></br>

  * HP-UX
  * AIX
  * OSX
  * Slackware
  * Solaris

  Slackware is the odd in the above list. HP-UX, AIX, OSX, Solaris are developed by HP, IBM, APPLE, Oracle respectively and all are UNIX variant. Slackware is a Linux Operating System.

* <b>Is Linux Operating system Virus free?</b></br>

  No! There doesn’t exist any Operating System on this earth that is virus free. However Linux is known to have least number of Viruses, till date, yes even less than UNIX OS. Linux has had about 60-100 viruses listed till date. None of them actively spreading nowadays. A rough estimate of UNIX viruses is between 85 -120 viruses reported till date.

* <b>Linux is which kind of Operating System?</b></br>

  * Multi User
  * Multi Tasking
  * Multi Process
  * All of the above
  * None of the above

  All of the Above. Linux is an Operating System which supports Multi User, Running a Number of Processes performing different tasks simultaneously.

* <b>Syntax of any Linux command is:</b></br>

  * command [options] [arguments]
  * command options [arguments]
  * command [options] [arguments]
  * command options arguments

  The correct Syntax of Linux Command is Command [options] [arguments].

* <b>Choose the odd one out.</b></br>

  * Vi
  * vim
  * cd
  * nano

  The odd one in the above list is cd. Vi, vim and nano are editors which is useful in editing files, while cd command is used for changing directory.

* <b>How would you swap the `stdout` and `stderr` of a command?</b></br>

  To swap `stdout` and `stderr` of a command, a third file descriptor is being created (in this case 3), which is assigned to the same target that `stderr` is pointed to (referenced by &2). Then `stderr` is pointed to the same target `stdout` is pointed to (&1). Finally, `stdout` is pointed back to where the newly created file descriptor is pointed (which is the same target `stderr` originally pointed to.)

* <b>How would you count every occurrence of the term “potato” in all the files appearing under the current directory, and its subdirectories, recursively?</b></br>

  `$ grep -orI potato . | wc -l` </br>
  To list every occurrence of the term “potato” on a separate line, one must run `grep -o potato <path>`. Adding the `r` flag to the command makes the search recursively process every file under the given path, and the `I` flag ensures that matches in binary files are ignored. In addition, the `w` flag can be included to match the exact term only, and ignore superstrings such as “potatoes”, and to make the search case-insensitive, the `i` flag can be added as well:

  `$ grep -iworI potato . | wc -l` </br>

  The number of lines yielded by this `grep` command is the number of occurrences of the desired term, which can then be counted by piping it into the `wc -l` command.

* <b>How would you write a shell script that prints all the additional arguments passed to it in reverse order?</b></br>

  ```BASH
  for (( i = ${#}; i > 0; i-- )); do
      echo ${!i}
  done
  ```
  The arguments are available as `$<n>`, where `n` is the position of the argument. For example, `$0` would give the name of the script, `$1` would give the first additional argument, `$2` the second, and so on. The total number of additional arguments is found in `$#`.

  A loop that starts at `$#` and ends at 1 can be used to print each additional argument in reverse order.

* <b>How would you write a shell script and ensure that only one instance of the script may run for every user? Strong atomicity is not required.</b></br>

  In Bash:
  ```BASH
  LOCKFILE=/tmp/lock-`whoami`
  if [ -e ${LOCKFILE} ] && kill -0 `cat ${LOCKFILE}`; then
    echo "Already running!"
    exit 1
  fi
  trap "rm -f ${LOCKFILE}; exit" INT TERM EXIT
  echo $$ > ${LOCKFILE}
  ```
  Start by determining a name for the lock file. In this case, the lock file is generated by suffixing a common name with the username of the current user.

  Then, check if the lock file exists and if the PID contained within the lock file is running. If it is, exit with a message.

  Create a trap to remove the lock file on a clean exit, or unclean exits (any exit with the signal INT or TERM).

  Finally, if the script has not exited yet, create the lock file, and store the PID of the current process ($$) in it.

* <b>What are shared, slave, private, and unbindable mountpoints?</b></br>

  * A mount point that is shared may be replicated as many times as needed, and each copy will continue to be the exact same. Other mount points that appear under a shared mount point in some subdirectory will appear in all the other replicated mount points as it is.

  * A slave mount point is similar to a shared mount point with the small exception that the “sharing” of mount point information happens in one direction. A mount point that is slave will only receive mount and unmount events. Anything that is mounted under this replicated mount point will not move towards the original mount point.

  * A private mount point is exactly what the name implies: private. Mount points that appear under a private mount point will not be shown elsewhere in the other replicated mount points unless they are explicitly mounted there as well.

  * An unbindable mount point, which by definition is also private, cannot be replicated elsewhere through the use of the bind flag of the mount system call or command.

* <b>What are some basic measures that you would take to harden a server’s SSH service?</b></br>

  There are a some very simple steps that can be taken to initially harden the SSH service, such as:

  * Forcing the service to use only version 2 of the protocol will introduce both security and feature enhancement.

  * Disabling root login, and even password-based logins, will further reinforce the security of the server.

  * The whitelist approach can be taken, where only the users that belong to a certain list can login via SSH to the server.

  * Disabling password-based login will require you to then allow key based logins, which is secure, but can be taken further by restricting their use from only certain IP addresses.

  * Changing the port to something other than 22 significantly decreases random brute force attempts from the internet.

  Sometimes the use of having an SSH service on a server may just be transferring files to and from the server (typically using tools like scp). In such a case, it is possible to change the shell of the user to something restrictive, such as [rssh](http://www.pizzashack.org/rssh/).

  Finally it is often desirable to know exactly what is going on while you are not logged into the server. The logging verbosity may be increased if needed. Often, it is the logs that allow one to figure out if a key has indeed been stolen and is being abused.

* <b>What is a Unix shell? Is Bash the only Unix shell?</b></br>

  A Unix shell is a software that provides a user interface for the underlying operating system. Unix shells typically provide a textual user interface - a command line interpreter - that may be used for entering and running commands, or create scripts that run a series of commands and can be used to express more advanced behavior.

  Bash is not the only Unix shell, but just one of many. Short for Bourne-Again Shell, it is also one of the many Bourne-compatible shells. However, Bash is arguably one of the most popular shells around. There are other, modern shells available that often retain backwards compatibility with Bash but provide more functionality and features, such as the Z Shell (zsh).

* <b>Where is the target path of a symlink stored? How are permission settings for symlinks handled?</b></br>

  The target path of a symlink is stored in an inode - the data structure used to store file information on disk.

  Typically, the permission settings of the symlink itself only control the renaming and removal operations performed on the symlink itself. Any operation that deals with the contents of the file linked to are controlled by the permission settings of the target file.

* <b>What are terminal multiplexers? What are some of their key features? What are some of the more popular ones currently available?</b></br>

  Terminal multiplexers enable several terminals to be created and controlled from a single screen or from a single remote session. The terminals and sessions can be detached and left running, even with the user logging off.

  Two of the more common ones available today are [GNU Screen](http://www.gnu.org/software/screen/) and [tmux](http://tmux.sourceforge.net/).

`Screen` enables you to connect to multiple remote servers without needing to open multiple terminal shells. Work can be preserved and a session detached, for example, to wait for the output of a long-running command. On subsequent reconnection, users can reattach to existing sessions or run new sessions. Sessions can also be shared among different users, which may be useful in audit or training scenarios.

Both `Screen` and `tmux` support split-screen functionality (to be more precise, tmux supports this and `Screen` supports it via a plugin). This allows, for example, running `tail` on a service’s log file in one part of the screen, and editing the configuration of that service, and restarting it if necessary, in another.

* <b>What would be a simple way to continuously monitor the log file for a service that is running?</b></br>

  Probably the simplest and most common way to do this would be by using the command:

  `tail -F $LOGFILE`
  where `$LOGFILE` is an environment variable corresponding to the path to the log file to be monitored.

  By default, the Linux tail command prints the last 10 lines of a given file to standard output. The `-F` option causes additional file content to be displayed in realtime as the file continues to grow. This yields a simple mechanism for monitoring services via their log files in close to realtime.

  Two other specific command line options of interest in this context are:

  * The `-s` option causes tail to sleep for a specified number of seconds between updates (e.g., `tail -F -s 10` will update the displayed file contents roughly every 10 seconds rather than in close to realtime as the file is updated).

  * The `-n` option can be used to specify a number of lines other than 10 to initially display (e.g., `tail -n 20 -F` will first display the last 20 lines of the file and will then continue updating the output in realtime).

* <b>What is a Linux null (or Blackhole) route? How can it be used to mitigate unwanted incoming connections?</b></br>

  A [Linux null (or Blackhole) route](http://bencane.com/2013/01/14/mitigating-dos-attacks-with-a-null-or-blackhole-route-on-linux/) is a type of routing table entry which, upon matching a packet, discards it without forwarding the packet any further or sending any ICMP.

  Using this technique, it is possible to block an IP (or range of IP addresses) by running a simple command. For example, blocking 192.168.0.1 can simply be done with the following command:

  `# ip route add blackhole 192.168.0.1/32`

* <b>Why should you periodically update the kernel and package versions?</b></br>

  To enhance the security of system you should ensure that you are using the latest versions kernel and software packages that contain the most recent security updates.

* <b>During a recent strikes at office, several archive tapes of the system were damaged and ruined. What can you do to prevent the physical damage in future?</b></br>

  You should store them at offsite.

* <b>Why should you avoid the Telnet to administer a Linux system remotely? </b></br>

  Telnet use most insecure method for communication. It send data across the network in plain text format. Someone easily find out the password using the network tool.

* <b>A file is unable to be restored from tape due to several device and media errors. What is most likely the cause?</b></br>

  Media errors usually indicate that the tape media is damaged, or that the tape drive heads need cleaning.

* <b>Your FTP Server recently hacked. Due to the amount of damage, the entire server needs to be restored. How should you restore the original kernel system files?</b></br>

You cannot restore the entire operating system from tap back up device. So you should reinstall the core operating system, and then restore system configuration files and user data from tape backup device.

* <b>Your company hire a contract employee for two months. What should the Linux administrator do to enhance security on the employee's account?</b></br>

While creating new user account for this user, administrator should set the expiration date for his account, so that if the employee leaves or does not have their contract renewed, the account will be automatically disabled.

* <b>Which backup strategy only backs up files that have changed since the last full backup?</b></br>

Differential backup will backup files that have changed since the last full backup.

* <b>Name a service which should you disable on a Linux Server which is acting as both a Web and FTP Server.</b></br>

The finger service should be disabled because a remote user can get important information about the system by using that command.

* <b>Why it is recommended to store backup tapes to an offsite storage facility?</b></br>

Because this will prevent the backup taps from being destroyed during a natural disaster at the server site. It also prevents the tapes from being stolen.

* <b>A newbie enabled the root session for FTP server. is it ok?</b></br>

No, he has put the security of entire server on risk. You should disable to root session as soon as possible.

* <b>A user complains you that he is unable to set '123' as his password. Why would not the system allow this password?</b></br>

There would be a minimum length rule for password, which is blocking user to use this password. Default minimum length rule for password is six characters. It means a user cannot have password less than six characters.

* <b>Your company is running Web Server. One dedicate account holder customer complains that his visitors are able to scan the directory tree. Which directive would you configure to stop web server from listing the directory?</b></br>

You should remove / comment the "Options Indexes" directive from the main configuration file ' httpd.conf' of the web server. This is a security measure so that remote users can’t scan the directory tree of the server looking for security holes. Server won’t show directory listings if requested by a user.

* <b>What type of backup strategy can you use to fully back up a system every night?</b></br>

You can use full backup strategy that will always perform a full backup of all files. This takes much more time and space than other methods, but is it the most complete method and allows for easy file restoration.

* <b>How can you enhance the security of password file?</b></br>

Linux keep user account information in a text file called /etc/passwd. This file also store one way encrypted password. This file is accessed by several tools to get user information, so file need to world readable. This is a security risk. To minimize the security risk you can use shadow password format. This method save account information in regular file /etc/passwd. However, the password is stored as a single "x" character (not actually stored in this file). A second file, called "/etc/shadow", contains encrypted password as well as other information such as account or password expiration values, etc. The /etc/shadow file is readable only by the root account and is therefore less of a security risk.

* <b>What command should be used to make a tar archive to a disk file system located in `/mnt/backup`?</b></br>

The correct command is `tar -cvf /mnt/backup`. The /mnt/backup directory should be on another machine to be fully effective as a backup strategy.

* <b>You have just finished the installation of sever. This server is going to be use as file server. Default installation have send mail service running, while this server will never send any e-mails. How should you deal with send mail service?</b></br>

You should disable the send mail service if server is not being used for mail purpose. Leaving them running can increase the chance of a security vulnerability being exploited, and unauthorized use of sendmail relay.

* <b>What command can you use to back up an entire file system most efficiently?</b></br>

The easiest command to use to back up an entire file system is the dump command. Files can be restored from a dump operation by using the restore command.

* <b>Which necessary steps should you take to enhance the security of server just after the initial installation?</b></br>

  * Kernel and packages should be upgraded to the latest versions.
  * Unnecessary services and daemons should be disable.
  * Enable and configure firewall
  * Set a complex password policy.

* <b>While auditing user accounts, an administrator notices that one of the users has a blank password. What should he do to the account?</b></br>

To prevent further use of the account, which is an immediate security risk, disable it and set a temporary password for the user for the next time they login.

* <b>Which backup strategy backs up all files that have changed since the last backup?</b></br>

An incremental backup will only back up files that have changed since the last backup.

* <b>Your company has terminated a server administrator. What is first thing as an administrator should you do to enhance the security?</b></br>

Because the server administrator knows the root password for the server, it should be changed immediately to prevent them from tampering with the system.

* <b>You are setting up an FTP server. Only company employees are allowed to use the FTP services. What should you configure on the FTP server to enhance security?</b></br>

You should disable the anonymous FTP account, so that only users with a username and password can access the system.

* <b>What is the location of system configuration files that should be backed up on a regular basis?</b></br>

The /etc directory contains most of the Linux system configuration files.

* <b>Which permission allows a user to run an executable with the permissions of the owner of that file?</b></br>

The Set-User-ID is a special permission that allows a user to run an executable with the permissions of the owner of that file.

* <b>What command can you use to make a tape archive file of a /home directory, and send it to the /dev/tape device?</b></br>

  The correct command is `tar -cvf /dev/tape /home`.

  The `-xvf` option is used to extract files from an archive.

* <b>Employees at your company are lazy in changing the password. As a system administrator what can you do to minimize the security risk?</b></br>

You can setup a password policy which enforce user to change his password after a specific time periods.

* <b>Which program should you use to connect a system remotely?</b></br>

You should always use SSH to connect a system remotely. SSH is a secure method that encrypts the entire session.

* <b>To save disk space, an administrator wants to backup files, and then remove them from the server permanently. What kind of backup operation is this?</b></br>

An archive operation will take the files, back them up to a device, and then remove the files from the original server.

* <b>What does firewall do?</b></br>

Firewall is a device or service which can be used to protect the network or system from other outside networks.

* <b>What is a command redirection operator in Linux?</b></br>

The command redirection operator is a special character which is used to control the input and output of a command in Linux.

* <b>Describe any five command redirection operators.</b></br>

  * > : Takes the output form the command specified before it and redirects that into the specified location after it

  * < : Takes input from the specified location after it and sends that into the command specified before it

  * >> : Takes the output from the command specified before it and appends that in the end of file specified after it

  * | : Takes the output from the command specified before it and sends that to the command specified after it as input

  * && : Executes the command specified after it once the command specified before it is executed

* <b>Why LVM is required?</b></br>

  LVM stands for Logical Volume Manager , to resize filesystem’s size online we required LVM partition in Linux. Size of LVM partition can be extended and reduced using the lvextend & lvreduce commands respectively.

* <b>How To check Memory stats and CPU stats?</b></br>

  Using ‘free’ & ‘vmstat’ command we can display the physical and virtual memory statistics respectively.With the help of ‘sar’ command we see the CPU utilization & other stats.

* <b>What does Sar provides and at which location Sar logs are stored?</b></br>

  Sar Collect, report, or save system activity information. The default version of the sar command (CPU utilization report) might be one of the first facilities the  user  runs  to  begin system  activity investigation, because it monitors major system resources. If CPU utilization is near 100 percent (user + nice + system), the workload sampled is CPU-bound.

  By  default log files of Sar command  is located at  /var/log/sa/sadd file, where the dd parameter indicates the current day.

* <b>How to increase the size of LVM partition?</b></br>

  Below are the Logical Steps :
  – Use the lvextend command (lvextend -L +100M /dev/<Name of the LVM Partition> , in this example we are extending the size by 100MB.
    – resize2fs /dev/<Name of the LVM Partition>
    – check the size of partition using ‘df -h’ command

* <b>How to reduce or shrink the size of LVM partition?</b></br>

  Below are the logical Steps to reduce size of LVM partition :
  -Umount the filesystem using umount command,
  -use resize2fs command , e.g resiz2fs /dev/mapper/myvg-mylv 10G
  -Now use the lvreduce command , e.g lvreduce -L 10G /dev/mapper/myvg-mylv

  Above Command will shrink the size & will make the filesystem size 10GB.

* <b>How to create partition from the raw disk?</b></br>

  Using fdisk utility we can create partitions from the raw disk.Below are the steps to create partition from the raw dsik :
  – fdisk  /dev/hd* (IDE) or /dev/sd* (SCSI)
  – Type n to create a new partition
  –  After creating partition , type w command to write the changes to the partition table.

* <b>Where the kernel modules are located?</b></br>

   The ‘/lib/modules/kernel-version/’ directory stores all kernel modules or compiled drivers in Linux operating system. Also with ‘lsmod’ command we can see all the installed kernel modules.

* <b>What is umask?</b></br>

  umask stands for ‘User file creation mask’, which determines the settings of a mask that controls which file permissions are set for files and directories when they are created.

* <b>How to set the umask permanently for a user?</b></br>

  To set this value permanently for a user, it has to be put in the appropriate profile file which depends on the default shell of the user.

* <b>How to change the default run level in linux?</b></br>

  To change the run level we have to edit the file “/etc/inittab” and change initdefault entry ( id:5:initdefault:). Using ‘init’ command we change the run level temporary like ‘init 3’ , this command will move the system in runlevl 3.

* <b>How to share a directory using nfs?</b></br>

  To share a directory using nfs , first edit the configuration file ‘/etc/exportfs’ , add a entry like
  ‘/<directory-name>  <ip or Network>(Options)’ and then restart the nfs service.

* <b>How to check and mount nfs share?</b></br>

  Using ‘showmount’ command we can see what directories are shared via nfs e.g ‘showmount -e <ip address of nfs server>’.Using mount command we can mount the nfs share on linux machine.

* <b>What are the default ports used for SMTP,DNS,FTP,DHCP,SSH and squid?</b></br>

  Service      Port
  SMTP          25
  DNS            53
  FTP             20 (data transfer) , 21 ( Connection established)
  DHCP         67/UDP(dhcp server) , 68/UDP(dhcp client)
  SSH            22
  Squid         3128

* <b>What is Network Bonding?</b></br>

  Network bonding is the aggregation of multiple Lan cards into a single bonded interface to provide fault tolerance and high performance. Network bonding is also known as NIC Teaming.

* <b>What  are the different modes of Network bonding in Linux?</b></br>

Below are list of modes used in Network Bonding :

  * **balance-rr or 0** – round-robin mode for fault tolerance and load balancing.
  * **active-backup or 1** – Sets active-backup mode for fault tolerance.
balance-xor or 2 – Sets an XOR (exclusive-or) mode for fault tolerance and load balancing.
  * **broadcast or 3** – Sets a broadcast mode for fault tolerance. All transmissions are sent on all slave interfaces.
  * **802.3ad or 4**  – Sets an IEEE 802.3ad dynamic link aggregation mode. Creates aggregation groups that share the same speed & duplex settings.
  * **balance-tlb or 5** –  Sets a Transmit Load Balancing (TLB) mode for fault tolerance & load balancing.
  * **balance-alb or 6** –  Sets an Active Load Balancing (ALB) mode for fault tolerance & load balancing.

* <b>How to check and verify the status the bond interface.</b></br>

  Using the command ‘cat /proc/net/bonding/bond0’ , we can check which mode is enabled and what lan cards are used in this bond. In this example we have one only one bond interface but we can have multiple bond interface like bond1,bond2 and so on.

* <b>How to check default route and routing table?</b></br>

  Using the Commands ‘netstat -nr’ and ‘route -n’ we can see the default route and routing tables.

* <b>How to check which ports are listening in my Linux Server?</b></br>

  Use the Command ‘netstat –listen’ and ‘lsof -i’

* <b>List the services that are enabled at a particular run level in linux server?</b></br>

  With the help of command ‘chkconfig –list | grep 5:on’ we can list all the service that are enabled in run level5. For other run levels just replace 5 with the respective run level.

* <b>How to enable a service at a particular run level?</b></br>

  We can enable a service using the Command ‘chkconfig <Service-Name> on –level 3’

* <b>How to upgrade Kernel in Linux?</b></br>

  We should never upgrade Linux Kernel , always install the new New kernel using rpm command because upgrading a kenel can make your linux box in a unbootable state.

* <b>How To scan newly asssigned luns on linux box without rebooting?</b></br>

  Here are two ways to scan newly assigned luns :
  * Method:1 if sg3 rpm is installed , then run the command ‘rescan-scsi-bus.sh’
  * Method:2 Run the Command ,  echo ” – – – ” ></br>
   `/sys/class/scsi_host/hostX/scan`

* <b>How  to find WWN numbers of HBA cards in Linux Server?</b></br>

  We can find the WWN numbers of HBA cards using the command ‘systool -c fc_host -v | grep port_name’

* <b>How to add & change the Kernel parameters?</b></br>

  To Set the kernel parameters in linux , first edit the file ‘/etc/sysctl.conf’ after making the changes save the file and run the command ‘sysctl -p’ , this command will make the changes permanently without rebooting the machine.

* <b>What is Puppet Server?</b></br>

  Puppet is an open-source & enterprise software for configuration management toll in UNIX like  operating system.  Puppet is a  IT automation software used to push configuration to its clients (puppet agents) using code. Puppet code can do a variety of tasks from installing new software, to check file permissions, or updating user accounts & lots of other tasks.

* <b>What are manifests in Puppet?</b></br>

  Manifests in Puppet are the files in which the client configuration is specified.

* <b>Which Command is used to sign requested certificates in Puppet Server?</b></br>

  ‘puppetca  –sign hostname-of-agent’ in (2.X)  & ‘puppet ca  sign hostname-of-agent’ in  (3.X)

* <b>At which location  Puppet Master Stores Certificates?</b></br>

   `/var/lib/puppet/ssl/ca/signed`

* <b>How to find all the regular files in a directory?</b></br>

  using the command ‘find /<directory -type f’.

* <b>What is load average in Linux?</b></br>

  Load Average is defined as the average sum of the number of process waiting in the run queue and number of process currently executing over the period of 1,5 and 15  minutes. Using the ‘top’ and ‘uptime’ command we find the load average of a Linux sever.

* <b>What is Linux?</b></br>

  Linux is an operating system based on UNIX and was first introduced by Linus Torvalds. It is based on the Linux Kernel and can run on different hardware platforms manufactured by Intel, MIPS, HP, IBM, SPARC, and Motorola. Another popular element in Linux is its mascot, a penguin figure named Tux.

* <b>What is the difference between UNIX and LINUX?</b></br>

Unix originally began as a propriety operating system from Bell Laboratories, which later on spawned into different commercial versions. On the other hand, Linux is free, open source and intended as a non-propriety operating system for the masses.

* <b>What is BASH?</b></br>

BASH is short for Bourne Again SHell. It was written by Steve Bourne as a replacement to the original Bourne Shell (represented by /bin/sh). It combines all the features from the original version of Bourne Shell, plus additional functions to make it easier and more convenient to use. It has since been adapted as the default shell for most systems running Linux.

* <b>What is Linux Kernel?</b></br>

The Linux Kernel is a low-level systems software whose main role is to manage hardware resources for the user. It is also used to provide an interface for user-level interaction.

* <b>What is LILO?</b></br>

LILO is a boot loader for Linux. It is used mainly to load the Linux operating system into main memory so that it can begin its operations.

* <b>What is a swap space?</b></br>

Swap space is a certain amount of space used by Linux to temporarily hold some programs that are running concurrently. This happens when RAM does not have enough memory to hold all programs that are executing.

* <b>What is the advantage of open source?</b></br>

Open source allows you to distribute your software, including source codes freely to anyone who is interested. People would then be able to add features and even debug and correct errors that are in the source code. They can even make it run better and then redistribute these enhanced source code freely again. This eventually benefits everyone in the community.

* <b>What are the basic components of Linux?</b></br>

Just like any other typical operating system, Linux has all of these components: kernel, shells and GUIs, system utilities, and an application program. What makes Linux advantageous over other operating system is that every aspect comes with additional features and all codes for these are downloadable for free.

* <b>Does it help for a Linux system to have multiple desktop environments installed?</b></br>

In general, one desktop environment, like KDE or Gnome, is good enough to operate without issues. It's all a matter of preference for the user, although the system allows switching from one environment to another. Some programs will work in one environment and not work on the other, so it could also be considered a factor in selecting which environment to use.

* <b>What is the basic difference between BASH and DOS?</b></br>

The key differences between the BASH and DOS console lie in 3 areas:

  * BASH commands are case sensitive while DOS commands are not;

  * Under BASH, / character is a directory separator and \ acts as an escape character. Under DOS, / serves as a command argument delimiter and \ is the directory separator

  * DOS follows a convention in naming files, which is 8 character file name followed by a dot and 3 characters for the extension. BASH follows no such convention.

* <b>What is the importance of the GNU project?</b></br>

This so-called Free software movement allows several advantages, such as the freedom to run programs for any purpose and freedom to study and modify a program to your needs. It also allows you to redistribute copies of software to other people, as well as the freedom to improve software and have it released for the public.

* <b>Describe the root account.</b></br>

The root account is like a systems administrator account and allows you full control of the system. Here you can create and maintain user accounts, assigning different permissions for each account. It is the default account every time you install Linux.

* <b>What is CLI?</b></br>

CLI is short for Command Line Interface. This interface allows the user to type declarative commands to instruct the computer to perform operations. CLI offers greater flexibility. However, other users who are already accustomed to using GUI find it difficult to remember commands including attributes that come with it.

* <b>What is GUI?</b></br>

GUI, or Graphical User Interface, make use of images and icons that users click and manipulate as a way of communicating with the computer. Instead of having to remember and type commands, the use of graphical elements makes it easier to interact with the system, as well as adding more attraction through images, icons, and colors.

* <b>How do you open a command prompt when issuing a command?</b></br>

To open the default shell (which is where the command prompt can be found), press Ctrl-Alt-F1. This will provide a command line interface (CLI) from which you can run commands as needed.

* <b>How can you find out how much memory Linux is using?</b></br>

  From a command shell, use the "concatenate" command: cat /proc/meminfo for memory usage information. You should see a line starting something like Mem: 64655360, etc. This is the total memory Linux thinks it has available to use.

  You can also use commands
```BASH
  free - m
  vmstat
  top
  htop
  ```
  to find current memory usage

* <b>What is a typical size for a swap partition under a Linux system?</b></br>

The preferred size for a swap partition is twice the amount of physical memory available on the system. If this is not possible, then the minimum size should be the same as the amount of memory installed.

* <b>What are symbolic links?</b></br>

Symbolic links act similarly to shortcuts in Windows. Such links point to programs, files or directories. It also allows you instant access to it without having to go directly to the entire pathname.

* <b>Does the Ctrl+Alt+Del key combination work on Linux?</b></br>

Yes, it does. Just like Windows, you can use this key combination to perform a system restart. One difference is that you won't be getting any confirmation message and therefore, a reboot is immediate.

* <b>How do you refer to the parallel port where devices such as printers are connected?</b></br>

  Whereas under Windows you refer to the parallel port as the LPT port, under Linux you refer to it as /dev/lp . LPT1, LPT2 and LPT3 would therefore be referred to as /dev/lp0, /dev/lp1, or /dev/lp2 under Linux.

* <b>Are drives such as hard drive and floppy drives represented with drive letters?</b></br>

  No. In Linux, each drive and device have different designations. For example, floppy drives are referred to as /dev/fd0 and /dev/fd1. IDE/EIDE hard drives are referred to as /dev/hda, /dev/hdb, /dev/hdc, and so forth.

* <b>How do you change permissions under Linux?</b></br>

Assuming you are the system administrator or the owner of a file or directory, you can grant permission using the chmod command. Use + symbol to add permission or – symbol to deny permission, along with any of the following letters: u (user), g (group), o (others), a (all), r (read), w (write) and x (execute). For example, the command chmod go+rw FILE1.TXT grants read and write access to the file FILE1.TXT, which is assigned to groups and others.

* <b>In Linux, what names are assigned to the different serial ports?</b></br>

Serial ports are identified as /dev/ttyS0 to /dev/ttyS7. These are the equivalent names of COM1 to COM8 in Windows.

* <b>How do you access partitions under Linux?</b></br>

Linux assigns numbers at the end of the drive identifier. For example, if the first IDE hard drive had three primary partitions, they would be named/numbered, /dev/hda1, /dev/hda2 and /dev/hda3.

* <b>What are hard links?</b></br>

Hard links point directly to the physical file on disk, and not on the pathname. This means that if you rename or move the original file, the link will not break since the link is for the file itself, not the path where the file is located.

* <b>What is the maximum length for a filename under Linux?</b></br>

Any filename can have a maximum of 255 characters. This limit does not include the path name, so therefore the entire pathname and filename could well exceed 255 characters.

* <b>What are filenames that are preceded by a dot?</b></br>

In general, filenames that are preceded by a dot are hidden files. These files can be configuration files that hold important data or setup info. Setting these files as hidden makes it less likely to be accidentally deleted.

* <b>Explain virtual desktop.</b></br>

This serves as an alternative to minimizing and maximizing different windows on the current desktop. Using virtual desktops can clear the desktop when you can open one or more programs. Rather than minimizing/restoring all those programs as needed, you can simply shuffle between virtual desktops with programs intact in each one.

* <b>How do you share a program across different virtual desktops under Linux?</b></br>

To share a program across different virtual desktops, in the upper left-hand corner of a program window look for an icon that looks like a pushpin. Pressing this button will "pin" that application in place, making it appear in all virtual desktops, in the same position onscreen.

* <b>What does a nameless (empty) directory represent?</b></br>

This empty directory name serves as the nameless base of the Linux file system. This serves as an attachment for all other directories, files, drives, and devices.

* <b>What is the pwd command?</b></br>

  The pwd command is short for print working directory command.

  Example:
  pwd
  Output:
  /home/guru99/myDir

* <b>What are daemons?</b></br>

Daemons are services that provide several functions that may not be available under the base operating system. Its main task is to listen for service request and at the same time to act on these requests. After the service is done, it is then disconnected and waits for further requests.

* <b>How do you switch from one desktop environment to another, such as switching from KDE to Gnome?</b></br>

Assuming you have these two environments installed, just log out from the graphical interface. Then at the login screen, type your login ID and password and choose which session type you wish to load. This choice will remain your default until you change it to something else.

* <b>What are the kinds of permissions under Linux?</b></br>

There are 3 kinds of permissions under Linux:- Read: users may read the files or list the directory- Write: users may write to the file of new files to the directory- Execute: users may run the file or lookup a specific file within a directory

* <b>How does case sensitivity affect the way you use commands?</b></br>

When we talk about case sensitivity, commands are considered identical only if every character is encoded as is, including lowercase and uppercase letters. This means that CD, cd, and Cd are three different commands. Entering a command using uppercase letters, where it should be in lowercase, will produce different outputs.

* <b>What are environmental variables?</b></br>

Environmental variables are global settings that control the shell's function as well as that of other Linux programs. Another common term for environmental variables is global shell variables.

* <b>What are the different modes when using vi editor?</b></br>

There are 3 modes under vi:- Command mode – this is the mode where you start in- Edit mode – this is the mode that allows you to do text editing- Ex mode – this is the mode wherein you interact with vi with instructions to process a file.

* <b>Is it possible to use shortcuts for a long pathname?</b></br>

Yes, there is. A feature known as filename expansion allows you do this using the TAB key. For example, if you have a path named /home/iceman/assignments directory, you would type as follows: /ho[tab]/ice[tab]/assi[tab] . This, however, assumes that the path is unique and that the shell you're using supports this feature.

* <b> What is redirection?</b></br>

Redirection is the process of directing data from one output to another. It can also be used to direct an output as an input to another process.

* <b>What is grep command?</b></br>

grep a search command that makes use of pattern-based searching. It makes use of options and parameters that are specified along with the command line and applies this pattern in searching the required file output.

* <b>What could be the problem when a command that was issued gave a different result from the last time it was used?</b></br>

One highly possible reason for getting different results from what seems to be the same command has something to do with case sensitivity issues. Since Linux is case sensitive, a command that was previously used might have been entered in a different format from the present one. For example, to lists all files in the directory, you should type the command ls, and not LS. Typing LS will either result in an error message if there is no program by that exact name exist or may produce a different output if there is a program named LS that performs another function.

* <b>What are the contents of /usr/local?</b></br>

It contains locally installed files. This directory matters in environments where files are stored on the network. Specifically, locally-installed files go to /usr/local/bin, /usr/local/lib, etc.). Another application of this directory is that it is used for software packages installed from source, or software not officially shipped with the distribution.

* <b>How do you terminate an ongoing process?</b></br>

Every process in the system is identified by a unique process id or pid. Use the kill command followed by the pid to terminate that process. To terminate all process at once, use kill 0.

* <b>How do you insert comments in the command line prompt?</b></br>

Comments are created by typing the # symbol before the actual comment text. This tells the shell to completely ignore what follows. For example "# This is just a comment that the shell will ignore."

* <b>What is command grouping and how does it work?</b></br>

You can use parentheses to group commands. For example, if you want to send the current date and time along with the contents of a file named OUTPUT to a second file named MYDATES, you can apply command grouping as follows: (date cat OUTPUT) > MYDATES

* <b>How do you execute more than one command or program from a single command line entry?</b></br>

  You can combine several commands by separating each command or program using a semicolon symbol. For example, you can issue such a series of commands in a single entry:

  ```
  ls –l cd .. ls –a MYWORK which is equivalent to 3 commands: ls -l cd.. ls -a MYWORK
  ```
  \*\*Note that this will be executed one after the other, in the order specified.

* <b>Write a command that will look for files with an extension "c", and has the occurrence of the string "apple" in it.</b></br>

  ```
  Find ./ -name "*.c" | xargs grep –i "apple"
  ```

* <b>Write a command that will do the following:</b></br>

  * look for all files in the current and subsequent directories with an extension c,v
  * strip the,v from the result (you can use sed command)
  * use the result and use a grep command to search for all occurrences of the word ORANGE in the files.
  ```
  Find ./ -name "*.c,v" | sed 's/,v//g' | xargs grep "ORANGE"
  ```
* <b>What, if anything, is wrong with each of the following commands?
a) ls -l-s </br>
b) cat file1, file2 </br>
c) ls - s Factdir
</b></br>

  Answers:
  a) there should be space between the 2 options: ls -l -s
  b) do not use commas to separate arguments: cat file1 file2
  c) there should be no space between hyphen and option label: ls –s Factdir


* <b>What is the command to calculate the size of a folder?</b></br>

To calculate the size of a folder uses the command `du –sh folder1`.

* <b>How can you find the status of a process?</b></br>

Use the command `ps ux`

* <b>How can you check the memory status?</b></br>

  You can use the command

  * free -m to display output in MB

  * free -g to display output in GB

* <b>Explain how to color the Git console?</b></br>

  To color the Git console, you can use the command git config—global color.ui auto. In the command, the color.ui variable sets the default value for a variable such as color.diff and color.grep.

* <b>How can you append one file to another in Linux?</b></br>

  To append one file to another in Linux you can use command `cat file2 >> file 1`. The operator >> appends the output of the named file or creates the file if it is not created. While another command `cat file 1 file 2 > file 3` appends two or more files to one.

* <b>Explain how you can find a file using Terminal?</b></br>

  To find a file you have to use a command, `find . –name "process.txt"` . It will look for the current directory for a file called process.txt.

* <b>Explain how you can create a folder using Terminal?</b></br>

  To create a folder, you have to use command mkdir. It will be something like these: `~$ mkdir Guru99`

* <b>Explain how you can view the text file using Terminal?</b></br>

  To view the text file, go to the specific folder where the text files are located by using the command cd and then type less filename.txt.

* <b> Explain how to enable curl on Ubuntu LAMP stack?</b></br>

  To enable curl on Ubuntu, first, install libcurl, once done use following command `sudo/etc/init .d /apache2 restart` or `sudo service apache2 restart`.

* <b>Explain how to enable root logging in Ubuntu?</b></br>

  The command which enables root logging is

  `#sudo sh-c 'echo "greater-show-manual-login=true" >>/etc/lightdm/lightdm.conf'`

* <b> How can you run a Linux program in the background simultaneously when you start your Linux Server?</b></br>

  By using nohup. It will stop the process receiving the NOHUP signal and thus terminating it you log out of the program which was invoked with. & runs the process in the background.

* <b>Explain how to uninstall the libraries in Linux?</b></br>

To uninstall the libraries in Linux, you can use command sudo apt-get remove library_name

* <b>What Is Linux And Why Is It So Popular?</b></br>

  Linux is an operating system based on UNIX and was first introduced by Linus Torvalds. Most servers use Linux as its Operating System. It runs on different hardware platforms manufactured by Intel, MIPS, HP, IBM, SPARC, and Motorola. Another striking element in Linux is its mascot, a penguin figure with name Tux.

  The popularity of Linux is mainly because of the following reasons.

  * It is free and open-source. We can download Linux for free and customize it as per our needs.
  * It is very robust and adaptable.
  * It accompanies with an immense amount of libraries and utilities.


* <b>What Is BASH?</b></br>

  BASH is a short form for Bourne Again Shell. Steve Bourne developed it as a replacement to the original Bourne Shell (represented by /bin/sh). It combines all the features from the original version of Bourne Shell, plus additional functions to make it easier and more convenient to use. Since then it has been adapted as the default shell for most running systems.

* <b>What Is The Core Of The Linux Operating System?</b></br>

  The core of the Linux operating system is Kernel. It is broken down into Shell, Command, Script, and Terminal. Shell is the Command Line Interpreter.

  A Command is an instruction given to the Computer by the user to perform a task. A Script is a collection of commands stored in a file, and Terminal is the CLI.

* <b>What Are The Basic Differences Between UNIX And Linux Operating Systems?</b></br>

  Linux is free and open-source software (allows programmers to program with Linux, not around it). Linus Torvalds and community developed its Kernel.

  UNIX, on the other hand, is a copyrighted name. Only big companies can access and use its copyright and name.

  For example, the products like IBMAIX, SunSolaris, and HP-UX are all UNIX-based Operating Systems.

* <b>What Is LILO?</b></br>

  LILO is a boot loader for Linux.

  It is used mainly to load the Linux operating system into main memory so that it can begin its operations.

* <b>What Is An INODE?</b></br>

  All files have its description stored in a structure called “inode”. It stores information about the size of the file, access and modification times, file permissions and so on.

  In addition to above, it also holds the pointer to the data blocks of the files and it is unique. In simple words, it is a unique number allocated to a file in UNIX-like OS.

* <b>What Is A Swap Space?</b></br>

  A swap space is a certain amount of space used by Linux to temporarily hold some programs that are running concurrently.

  It is useful when RAM does not have enough available memory to hold all the programs that are executing at the same time. This space gets free when the execution of the program is complete.

* <b>What Is The Advantage Of Using An Open Source Software?</b></br>

  Open source allows you to distribute your software including the source code, freely to anyone who is interested. Anyone can help by adding new features to the software and can even debug and correct errors present in the source code.

  They can even make it run better and then redistribute the enhanced source code freely again. In this way, open-source benefits everyone in the community.

* <b>What Are The Key Differences Between BASH And DOS?</b></br>

  Following are the main differences between both the Console.

  * BASH commands are case-sensitive while DOS commands are not.
  * Under BASH, /character is a directory separator and acts as an escape character. Under DOS, /serves as a command argument delimiter and is the directory separator.
  * DOS follows a naming convention for files, where it allows maximum 8 characters of filename followed by a dot and then 3 characters for the extension. However, BASH follows no such convention.

* <b>What Are The Differences Between TCP And UDP?</b></br>

  The main differences between the two are as follows.

  * TCP stands for Transmission Control Protocol. It first establishes the connection before sending data and thus called as connection-oriented protocol. It controls the flow of data and also guarantees the delivery of packets.
  * UDP stands for User Datagram Protocol. It simply sends datagrams on to the wire. There is no ordering of packets, if some of the packets get lost in the way or they arrive in bad order then there is no way to request those packets again. Thus it is called as connection-less protocol. Some services like DNS resolution, SNMP, DHCP, RIP, and VOIP prefer to use UDP for its speed due to less network overhead. Any errors that occur during data transfer gets handled on the application layer rather than the network layer.

* <b>How Does DNS Resolution Determine The IP Address?</b></br>

  A client application requests an IP address from the name server usually by connecting to UDP port 53. The nameserver will attempt to resolve the FQDN based on its resolver library, which may contain authoritative information about the host requested or cached data about that name from an earlier query.

  If the nameserver does not already have the answer, it will turn to root nameservers to determine the authoritative for the FQDN in question. Then, with that information, it will query the authoritative nameservers for that name to determine the IP address.

* <b>Describe What Is A Root Account In Linux?</b></br>

  It is like a system administrators account that grants full control on the system. It allows creating and maintaining user accounts and assigning different permissions for each account, has access to all commands and files on the system. It is the default account that gets created at every new installation of Linux.

  We can refer to it as the root user or a super user. There is a special command named <su> (for “super user”, or “switch user”) that allows to switch over to the root account on the command line. If you enter the correct root password, you enter into the root account to execute commands with full system privileges.

* <b>Which Linux Command Do You Use To Check The Memory Available For Use?</b></br>

  From a command shell, execute the concatenate command to provide the memory usage information.

  `cat /proc/meminfo`
  This command displays the following output on the terminal.

  `Mem:  64655360`
  This output tells about the total memory available for use.

* <b>What Do You Know About The MX Record?</b></br>

  MX (Mail eXchanger) records are like an address for your domain’s email. It tells the rest of the internet about the mail server responsible for accepting email messages on behalf of a recipient’s domain.

  It is also a kind of preference value which determines the server for processing the mail delivery if multiple servers are available. This number can assume any value between 0 to 65535.

  The MX record with the lowest number will have more weightage over the others. The user can also set multiple e-mail servers with the same preference value for load balancing.

* <b>What Are The Steps That Define The Linux Boot-Up Sequence?</b></br>

  There are seven steps in the boot-up sequence.

  * BIOS (basic input/output system) – Executes the MBR where Boot Loader sits.
  * MBR – Master boot reads Kernel into memory.
  * GRUB(Grand Unified Bootloader)- Kernel starts Init process.
  * Kernel – It executes the </sbin/init> program. Then, the init process reads <inittab> file and executes the <rc.sysinit>.
  * The init script – It is the <rc> script to start services for reaching the default run level.
  * Run level programs – These programs execute from the </etc/rc.d/rc*.dl>.


* <b>What Is The Recommended Size For A Swap Partition Under A Linux System?</b></br>

  The standard size for a swap partition is twice the amount of physical memory available on the system.

  If this is not possible, then the minimum size should be the same as the amount of memory installed.

* <b>How Do You Search For A Pattern And Then Replace It In An Entire File?</b></br>

Linux provides <sed> command and <vi-editor> to perform “search and replace” action for a pattern.

  1. Using Sed Command.
  The sed command searches for a particular pattern in the file. And if a match occurs, then it replaces the text with the target string mentioned in the command.
  Syntax for sed “Search and Replace”-

  sed 's/SEARCH/REPLACE/OPTIONS' FILE.txt
  where,

  * “s” is used to search for a pattern.
  * “/” – It’s a delimiter. There are some alternatives for / like # % @ :.
  * SEARCH – mention the search pattern here.
  * REPLACE – define the string that will replace the search pattern.
  * OPTIONS – This command comes with the following options.
    * <g> – Helpful when the user requires replacing ALL the SEARCH instances with REPLACE string.
    * <i> – To search a pattern in case insensitive mode.
    * <n> – Unlike option <g>, <n> requires replacing only the nth occurrence of the search pattern.
    * <p> – prints only the line containing the search pattern.
    * <w> – To edit the original file, you may use option <i>. But, in case you want to write the output to another file, keeping the original file intact, you can use option <w>. Using redirection operators (> or >>) is another way.


  2. Using Vi Editor.
  vi also has a powerful search and replace capabilities. For searching any string in a file, just type a colon (:), “s”, forward slash (/) and the search string in the command mode of the vi editor. What we type will appear on the bottom line of the display screen.
  On pressing ENTER, the area containing the matching text will get highlighted, if it exists.

  The formal syntax for searching is:

  `:s/string`
  The syntax for replacing one string with another string in the current line is:

  `:s/search pattern/replace string/`
  Following is the command to replace all the occurrences of the search string in the entire text. You have to add a “%” in front of the “s” as:

  `:%s/search pattern/replace string/`

* <b>How Does The Following Key (Ctrl+Alt+Del) Combination Work In Linux?</b></br>

  Yes, it works in Linux just like Windows. This key combination when used performs a system restart.

  The only difference is that no confirmation pop-up occurs and therefore the reboot is immediate.

* <b>How Do You Perform The List And Flush Of All IP Tables?</b></br>

  First, you use the –L  switch to view all the currently present rules and then –F to flush them.

* <b>How Do You Change Permissions In Linux?</b></br>

  A system administrator or the owner of a file or directory can grant permission using the <chmod> command.

  User adds permission to a file using “+” symbol and denies permission using “–” symbol, along with one or more of the following letters.

  * -u(user),
  * -g(group),
  * -o(others),
  * -a(all),
  * -r(read),
  * -w(write), and
  * -x(execute).

  For example the command.

  `chmod go+rw FILE1.TXT`
  It grants read and write access to the file FILE1.TXT, which is accessible to both groups and others.

* <b>What Is A Shell? List The Name Of Different Shells Available In Linux.</b></br>

  Shell is a user program or it’s environment provided for user interaction. It is a command language interpreter that executes the commands read from the standard input device like a keyboard or from a file.

  Shell is not part of the system kernel but uses the system kernel to execute programs and create files.

  Following Shells are available with Linux SH, BASH, CSH, TCSH, and KSH. Other functions of a shell include scripting capability, the path memory, multitasking, and file handling.

* <b>In Linux, What Names Are Assigned To The Different Serial Ports?</b></br>

  Serial ports are identified as /dev/ttyS0 to /dev/ttyS7.

  These are the names equivalent to COM1 to COM8 in Windows.

* <b>What Is A Zombie Process?</b></br>

  Zombies are essentially the premature processes whose mature parent processes died without reaping its children. Zombie processes are already dead.

  The kill command or system call has no effect on it. It’s just an entry in the process table. None of the resources like memory, running code or any active file does have any association with a zombie.

* <b>What Makes A Process A Zombie?</b></br>

  When a process dies, all resources are cleaned up including the entry in the process table. This entry is kept around, forming a zombie, to allow the parent process to track the exit status of the child.

  The parent determines the exit status by calling wait() syscall. Calling wait() drives the zombie to disappear and this means reaping the child. Thus we can say that a zombie comes into existence when a process dies, but its parent hasn’t called wait yet.

* <b>How Can We See If There Are Zombie Processes On A System?</b></br>

  An existing zombie process can be determined by running “ps aux” and then looking for a Z in the STAT column.

* <b>How To Remove The Zombie Process From A System?</b></br>

  There are two ways to terminate a zombie.

  * If the parent is alive, then it must call a wait() syscall to clean up a zombie.
  * In the other case, if the parent dies before the child or dies without reading the child’s status, the zombie’s parent process is set to <init> (the process with PID 1). Now, the <init> has to ensure to call the wait() for the occupied zombie process.

* <b>How Do You Access Partitions Under Linux?</b></br>

  Linux assigns numbers at the end of the identifiers assigned to drives.

  For example, if the first IDE hard drive had three primary partitions, they would be named/numbered as </dev/hda1>, </dev/hda2>, and </dev/hda3>.

* <b>What Is The Purpose Of ‘Hash’ Command?</b></br>

  The “hash” is one of a bash shell’s built-in command. It makes use of a hash table to keep the list of pathnames for the commands executed in the shell. Whenever you run any command, the shell starts searching for it in the variable $PATH.

  However, if the command is present in the hash table, then the Shell picks it from there for execution. The hash table stores all the entrances of each command used so far in that shell.

  For Example.
  ```BASH
  $ hash
  hits    command
  1    /usr/bin/cat
  2    /usr/bin/ps
  4    /usr/bin/ls
  ```
  You can delete a particular command from a hash table using -d option, and -r option to reset the complete hash table.
  ```BASH
  $ hash -d cat
  $ hash
  hits    command
  2    /usr/bin/ps
  4    /usr/bin/ls
  ```

* <b>What Is A Virtual Desktop?</b></br>

  It serves as an alternate to the action of minimizing and maximizing of different windows that need to focus on the current desktop. Every desktop that uses this feature behaves like a clean slate where you can open one or more programs.

  It is simple to shuffle between virtual desktops keeping the programs intact in each one of them. Rather than, minimizing/restoring these programs again and again while focusing on them.

* <b>How Will You Share A Program Across Different Virtual Desktops Under Linux?</b></br>

  There is an icon present in the upper left-hand corner of the program window that looks like a pushpin. e.g. In Ubuntu.

  On pressing this button, the application will get pinned, causing it to appear on all virtual desktops and in the same position on their screen.

* <b>Read More</b></br>

  * [10 Job Interview Questions for Linux System Administrators from Linux.com](https://www.linuxfoundation.org/blog/2015/07/10-job-interview-questions-for-linux-system-administrators/)
  * [10 Useful Random Linux Interview Questions and Answers](http://www.tecmint.com/useful-random-linux-interview-questions-and-answers/)
  * [11 Basic Linux Interview Questions and Answers](http://www.tecmint.com/basic-linux-interview-questions-and-answers/)
  * [11 Essential Linux Interview Questions from Toptal](http://www.toptal.com/linux/interview-questions)
  * [Some basic Linux questions from ComputerNetworkingNotes.com](http://computernetworkingnotes.com/rhce-interview-questions/linux-interview-questions-answers.html)
  * [Top 30 Linux System Admin Interview Questions & Answers](http://www.linuxtechi.com/experience-linux-admin-interview-questions/)
  * [Top 50 Linux Interview Questions from Career Guru](http://career.guru99.com/top-50-linux-interview-questions/)
  * [Linux System Administrator/DevOps Interview Questions](https://github.com/chassing/linux-sysadmin-interview-questions)
  * [278 Test Questions and Answers for \*nix System Administrators](https://github.com/trimstray/test-your-sysadmin-skills)
  * [Linux Interview Questions - Quick Refresher](https://www.techbeamers.com/essential-linux-questions-answers/)

### Windows

* <b>Pretend I’m a manager, and explain DNS to me.</b></br>

  Windows is increasingly tied to domain name resolution, and the bigger your company gets, the thornier DNS problems become.  If they can verbalize how end users’ computers make DNS requests and how forwarders work, and then if they can toss in Active Directory, they’ve solved some enterprise problems.

  Starting with a generic open-ended question like that tests a candidate’s communication skills, too.  Bonus points for making a tough concept seem easy.

* <b>What’s a Windows profile? When would you delete one, and what gets deleted?</b></br>

  If you’re looking for someone to do desktop support, they should have at least a vague idea of where the user’s data can be stored.  Bonus points if they can explain where common application settings are stored, what the Registry is, and how roaming profiles work.

* <b>When an end user says a file went missing, what do you do?</b></br>

  End users delete files all the time, but before you recover it from backup, first do a search on the drive to make sure they didn’t drag & drop it to another folder.  (Normally I don’t give interview answers here, but that one’s an exception.)  Then, after they explain that, I’d ask them to cover things like VSS snapshots, end user recovery in Explorer and how to restore from their favorite backup program.

* <b>How do you recover one SQL Server database or one Exchange mailbox?</b></br>

  Different backup systems have different ways of dealing with this, so I may not be able to vet their exact answer if I haven’t used the same backup system they’re using.  However, I can do a pretty good job of sniffing out when someone doesn’t understand the complexities involved.  If they shrug and just say “I click restore and it’s done,” then they’re bluffing.

  For example, when restoring an Exchange mailbox, do you really want to pave over every email the user has received since the last backup?  Or does the user just need one or two important emails pulled out of the archive?

* <b>If you get hired and you can pick any laptop, what do you get?</b></br>

  I wanna see ’em get all excited.  I wanna see ’em giddy with glee at the thought of picking out their own shiny new hardware.  The more excited they get, the more I know systems administration is a way of life for them, not just a hobby.

* <b>What’s the first software you’d install?</b></br>

  Hardcore sysadmins have their own favorite tools they like to use.  Listen with an open mind, too – the more sysadmins you interview, the more cool tools you’ll discover.  If they mention a tool you haven’t used before, drill into it.  Find out why they use it and how it saves them time.  If it’s a tool they’re passionate enough to mention, then they can probably describe some underlying concepts and technologies involved, and it’ll give you more confidence that they know what they’re doing.

* <b>What do the letters PST mean to you?</b></br>

  I want to know if they’ve experienced the pains (both technical and legal) involved with these files.  How do they back up PST files if the end user leaves their laptop online all the time?  Are there any size concerns with PST files?  Is there a good way to use PSTs?

* <b>What’s PowerShell, and how do you feel about it?</b></br>

  I don’t necessarily need PowerShell experience (although it’s a big plus for Windows sysadmins) but I want to know that they’re at least vaguely aware of the concept and what it means.  Bonus points if they can relate scripting to the \*nix world, and if they bring up Windows Core.

* <b>Are you involved with any local user groups?</b></br>

Be it Windows or just a hardware hacker group, I love candidates who love communities.  I like seeing someone get so involved in what they do that they seek out other people who share similar interests.

* <b>What do you want to do next?</b></br>

Windows systems administration is a cool gateway into a lot of different careers.  Do they want to manage Exchange?  Become a SQL Server DBA?  Go into management to be the next CIO?  Having a drive and a passion means they’ll try to do a better job so they can keep moving up the ladder.

* <b>Explain what is Windows Server?</b></br>

Window server is a series of server operating system developed by Microsoft Corporation.

* <b>Explain in windows DNS server what is Primary, Secondary and Stub zone?</b></br>

  In windows DNS server,

  * Primary Zone: In this, the file is saved as normal text file with filename (.dns).

  * Secondary Zone: It maintains a read-only copy of zone database on another DNS server.  Also, it acts as a back-up server to the primary server by providing fault tolerance and load balancing

  * Stub Zone: It consists of a copy of name server and SOA records which is used for reducing the DNS search orders.

* <b>Explain what does IntelliMirror do?</b></br>

IntelliMirror helps to reconcile desktop settings, applications and stored files for users especially for those users who move between workstations or those who works offline.

* <b>In the case when MSI file is not available, how you can install an app?</b></br>

To add the application using the Software Installer.ZAP text file can be used rather than the windows installer

* <b>Explain how you can set up remote installation procedure without giving access to user?</b></br>

To do that, you have to go to,

gponameà  User Configuration à Windows Settings à Remote Installation Services à Choice Options

* <b>What does it mean by “tattooing” the Registry?</b></br>

“ Tattooing” the registry means user can modify and view user preference that are not stored in the maintained portions of the Registry.  Even if the group policy is changed or removed, the user preference will still persist in the registry.

* <b>Mention how many types of queries DNS does?</b></br>

  The types of queries DNS does are

  * Iterative Query
  * Recursive Query

* <b>Explain what is the primary function of the domain controller?</b></br>

  Primary function of the domain controller is to validate users to the networks, it also provide a catalog of Active Directory Objects.

* <b>What information is required when TCP/IP is configured on Window Server?</b></br>

To configure a TCP/PI client for an IPv4 client, you have to provide the IP address and the subnet mask.

* <b>Explain what does it mean caching only server in terms of DNS?</b></br>

The caching only DNS server provides information related to queries based on the data it contains in its DNS cache.

* <b>Explain what is the way to configure the DHCP server such that it allocates the same IP address to certain devices each time the address is removed?</b></br>

To configure the DHCP server, you can create a reservation for the device.  To create a reservation, you must know the MAC hardware address of the device.  To determine the MAC address for a network device you can use the ipconfig or nbs tat command line utilities.

* <b>Explain what is LDAP?</b></br>

To look up for the information from the server, e-mail and another program follows or uses the internet protocol. This protocol is referred as LDAP or Lightweight Directory Access Protocol.

* <b>Explain what is SYSVOL folder?</b></br>

It is a set of files and folders that is stored on the local hard disk of each domain controller in a domain and are replicated by the FRS ( File Replication Service).  These files contain group or user policy information.

* <b>Explain what is the difference between a thread and a computer process?</b></br>

  **Computer Process**: In computing, a process is an instance of a computer program that is executed sequentially by a computer system which can run several computer programs concurrently.

  **Thread**: A thread is a several executable program that work together as a single process.  For instance, one thread might send an error message to the user; another might handle error signals while the third thread might be executing the original action.

* <b>Explain what is RAID in Windows Server?</b></br>

For storing same data at a different place RAID or Redundant Array of Independent Disks strategy is used. It is a strategy for building fault tolerance and increase the storage capacity. On separate drives it allows you to combine one or more volumes so that they are accessed by a single drive letter

* <b>Explain what is the purpose of deploying local DNS servers?</b></br>

A local DNS server provides the local mapping of fully qualified domain names to IP addresses.  To resolve remote requests related to the domains names on your network, local DNS servers can provide record information to remote DNS servers.

* <b>To check TCP/IP configurations and IP connectivity, what are the two command line utilities that can be used?</b></br>

  **Ipconfig:** To check the computer’s IP configuration, command ipconfig can be used and also it can be used to renew the client’s IP address if it is provided by a DHCP server.

  **Ping:** To check the connection between the local computer and any of the other computer device on the network Ping command is used

* <b>Explain if it is possible to connect Active Directory to other 3rd party Directory services?</b></br>

Yes, you can connect other vendors directory services with Microsoft version.  By using dirXML or LDAP to connect to other directories.

* <b>Explain where is the AD database is held?</b></br>

  AD database is saved in %systemroot%/ntds.  Files that controls the AD structure are

  * ntds.dit
  * edb.log
  * res1.log
  * res2.log
  * edn.chk

* <b>Explain what is the major difference between NTFS ( New Technology File System) or FAT (File Allocation Table) on a local server?</b></br>

For local users FAT (File Allocation Table) and FAT32 provides security, while NTFS ( New Technology File System) provides security for domain users as well as local users.  NTFS provides file level security which is not possible through FAT32.

* <b>Mention what windows server 2008 service is used to install client operating system over the network?</b></br>

WDE ( Windows Deployment Services ) allows you to install client and server operating systems over the network to any computer with a PXE enabled network interface

* <b>Read more:</b></br>

  * [Top 10 Interview Questions for Windows Administrators](http://www.brentozar.com/archive/2009/07/top-10-interview-questions-for-windows-sysadmins/)
  * [Top 22 Windows Server Interview Questions from Career Guru](http://career.guru99.com/top-22-windows-server-interview-questions/)
  * [Windows Admin Interview Questions & Answers](http://www.01world.in/p/windows.html)


### Read More
