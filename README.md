== Description

apache-top provides real-time display of the active processes from a remote apache server. I’ts like the top linux command.

With apache-top you can get:

* The active apache processes with their associated PID, the status, the seconds being active, the CPU usage, the asociated VirtualHost, the accessing ip and the request (POST or GET, the file being accessed and the used protocol)
* The server uptime and the last time it was restarted
* The CPU usage
* Requests by second, Kb by second and the average Kb by request
* Number of active and inactive processes
* A graph with the inactive and active processes and their status

== Requeriments

* python 2.4
* Apache 2.0 webserver with mod_status and the ExtendedStatus directive activated. You will also need to be allowed to access from your ip address.

== Links

* http://www.fr3nd.net/projects/apache-top/
* https://github.com/fr3nd/apache-top

