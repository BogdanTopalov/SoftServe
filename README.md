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
2. Extract all ip addresses(ipv4 and ipv6) assigned to the host from ifconfig output. 
3. Present them in alphabetical order.

...

## Task 3
From http://www.almhuette-raith.at/apache-log/access.log:
1. Parse “access.log” file - find all unique IP addresses.
2. Group this IPs and sort them.
3. Calculate how much requests being made for each IP.

...

## Task 4
**Write a bash script to check:**
* Number of CPU cores
* Disk Space
* Size of RAM
* Provide information about the last logged users
* Number of active python processes

**Create a cron job which will send a report information on email address.**

...
