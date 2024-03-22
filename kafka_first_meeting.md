# First contact
Server Environment: 
  - kafka:3.7.0
  - os: opensuse
  - hostname: opensuse
Client Environment:
  - python & console-producer
  - os: mac
I'm trying to connect to kafka server about a whole afternoon.
It does no provide error info in python.
While using telnet to detect port, thus it is opened, 
but I can not send any data.
In python it is waiting all the time, and telnet will disconnect by server.

Finally I give console-producer a try, 
the error is java:unknow host name.
So I edit /etc/hosts file on client(mac book) to add ip_addr opensuse and it worked.
What the fuck!!!
I've tried at /etc/hosts ip_addr kafka-opensuse,
however it is the same issue: unknow host name, 
so the server name in /etc/hosts must be the same of real server host name.
