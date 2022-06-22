# SoftServe Linux Tasks

## Task 1
**Create regex for:**
1. Current time in fromat (hours:minutes:seconds) -> **[0-9]+:[0-9]+:[0-9]+**
    * **Command:** date | grep -E "above regex"
    * Example:

[![date-Linux.jpg](https://i.postimg.cc/25c2zN6t/date-Linux.jpg)](https://postimg.cc/B8Fxgy25)


2. Ipv4 address -> **[0-9][0-9]*\.[0-9][0-9]*\.[0-9][0-9]*\.[0-9][0-9]*$**
    * **Command:** grep -E "above regex" file-with-ip-addressese.txt

3. Paragraph of text -> **^$\n\_.\{-}\n$**
    * **Command:** grep -E "above regex" textfile.txt


## Task 2
1. Extract from 'ps' output pids of all the processes run from the current user.
   * **ps -A -o pid,cmd**
   * [![processes.jpg](https://i.postimg.cc/L4TzXQcB/processes.jpg)](https://postimg.cc/0rz6Xn2b)
2. Extract all ip addresses(ipv4 and ipv6) assigned to the host from ifconfig output. 
   * ...
3. Present them in alphabetical order.
   * ...

...

## Task 3
From http://www.almhuette-raith.at/apache-log/access.log:
1. Parse “access.log” file - find all unique IP addresses. -> ...
2. Group this IPs and sort them. -> ...
3. Calculate how much requests being made for each IP. -> ...

...

## Task 4
**Write a bash script to check:**
* Number of CPU cores
   * **nproc --all** or **lscpu** to see full info
   * [![cpu-Number.jpg](https://i.postimg.cc/VNGSj2FX/cpu-Number.jpg)](https://postimg.cc/bGnNPCWv)
* Disk Space
   * **df -h** or **df -h 'disc path'**
   * [![disk-Usage.jpg](https://i.postimg.cc/2SLn8kdg/disk-Usage.jpg)](https://postimg.cc/nXZX3tP1)
* Size of RAM
   * **grep memtotal /proc/meminfo**
   * [![ram.jpg](https://i.postimg.cc/7689yCpB/ram.jpg)](https://postimg.cc/Y4RY6S2g)
* Provide information about the last logged users
   * **last | head -n 1**
   * [![last-Login.jpg](https://i.postimg.cc/Wb6QYVJL/last-Login.jpg)](https://postimg.cc/F7zW12ZD)
* Number of active python processes
   * ...

**Create a cron job which will send a report information on email address.**

...
