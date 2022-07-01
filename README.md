# SoftServe Linux Tasks

## Task 1
**Create regex for:**
1. Current time in format (hours:minutes:seconds) -> **[0-9]+:[0-9]+:[0-9]+**
    * **Command:** date | grep -oE "above regex"

2. Ipv4 address -> **[0-9][0-9]*\.[0-9][0-9]*\.[0-9][0-9]*\.[0-9][0-9]*$**
    * **Command:** grep -oE "above regex" file-with-ip-addressese.txt

3. Paragraph of text -> **(?<=^|\n).+?$**
    * **Command:** grep -E "above regex" textfile.txt

**Bash script:**
   * [![task-01-bash.jpg](https://i.postimg.cc/ydw8spbb/task-01-bash.jpg)](https://postimg.cc/phJHBCxf)  

**Output:**
   * [![task-01-output.jpg](https://i.postimg.cc/1tgG3t95/task-01-output.jpg)](https://postimg.cc/9RhRxcRv)


## Task 2
1. Extract from 'ps' output pids of all the processes run from the current user.
   * **ps -A -o pid,cmd**
2. Extract all ip addresses(ipv4 and ipv6) assigned to the host from ifconfig output and present them in alphabetical order.
   * **ifconfig | grep inet[^6] | sort | awk '{print $2}'**
   * **ifconfig | grep inet6 | sort | awk '{print $2}'**

**Bash script:**
   * [![task-02-bash.jpg](https://i.postimg.cc/G2jGhSNz/task-02-bash.jpg)](https://postimg.cc/jwLLMvRJ)

**Output:**
   * [![task-02-output.jpg](https://i.postimg.cc/v8qxq9d1/task-02-output.jpg)](https://postimg.cc/Cd8KdR5Y)


## Task 3
From http://www.almhuette-raith.at/apache-log/access.log:
1. Parse “access.log” file - find all unique IP addresses. -> ...
2. Group this IPs and sort them. -> ...
3. Calculate how much requests being made for each IP. -> ...

...

## Task 4
**Write a bash script:**
* Number of CPU cores
   * **nproc --all** or **lscpu** to see full info
* Disk Space
   * **df -h** or **df -h 'disc path'**
* Size of RAM
   * **grep memtotal /proc/meminfo**
* Provide information about the last logged user
   * **last | head -n 1**
* Number of active python processes
   * ...
* Create a cron job which will send a report information on email address.
   * ...

**Bash script:**
   * [![task-04-bash.jpg](https://i.postimg.cc/RFFQthGH/task-04-bash.jpg)](https://postimg.cc/WDBkL2BN)  

**Output:**
   * [![task-04-output.jpg](https://i.postimg.cc/3Rgw151F/task-04-output.jpg)](https://postimg.cc/62pw6PD8)
