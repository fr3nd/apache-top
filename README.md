Description
===========

apache-top provides real-time display of the active processes from a remote apache server. I’ts like the top linux command.

With apache-top you can get:

* The active apache processes with their associated PID, the status, the seconds being active, the CPU usage, the asociated VirtualHost, the accessing ip and the request (POST or GET, the file being accessed and the used protocol)
* The server uptime and the last time it was restarted
* The CPU usage
* Requests by second, Kb by second and the average Kb by request
* Number of active and inactive processes
* A graph with the inactive and active processes and their status

Requirements
============

* python 2.4
* python-curses package
* Apache 2.0 webserver with mod_status and the ExtendedStatus directive activated. You will also need to be allowed to access from your ip address.

Examples
========

To see statistics from the webserver 192.168.0.1:

    apache-top -u http://192.168.0.1/server-status

If for any reason we don’t have direct access to 80 port, a tunel can be created using ssh:

    ssh -L 8080:localhost:80 192.168.0.1

And we run this command in other terminal:

    apache-top -u http://localhost:8080/server-status

Links
=====

* http://www.fr3nd.net/projects/apache-top/
* https://github.com/fr3nd/apache-top

