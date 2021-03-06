Author: Ashley Cawley // @ashleycawley

This script is designed to get the client computer (Raspberry Pi) to publish
its status to a central (web) server, with the idea of multiple different systems
all publishing their status to that central server so that the Administrator has
one easy place to view the general health and uptime of the systems or IOT devices.

An example of some of data the client system would publish would be: Hostname,
Uptime, Load, Users logged on, LAN & WAN IP's, MAC Address, CPU & GPU temperatures,
Free disk space and more.

The Bash script contains a self-installer, it checks to see if it is already present
in /usr/local/bin and if it is not then it copies itself to that location and then
installs an entry in the crontab to trigger itself on a regular basis (eg. hourly).
