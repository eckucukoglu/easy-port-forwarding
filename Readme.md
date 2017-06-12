# mercury port forwarding

Scripts to ease application-level port forwarding. Under favour of OpenSSH SSH client, allocates a socket to listen to port **8080** on the local side. Whenever a connection is made to this port, the connection is forwarded over the secure channel, and the application protocol is then used to determine where to connect to from the remote machine.

Port **22** is used to connect to on the remote host.
## Commands
To use, just type mercury then double tab to autocomplete on command shell.

* **mercury-start-tunnel**: starts port-forwarding.
* **mercury-kill-tunnel**: kills existing port-forwarding.
* **mercury-check-tunnel**: checks and returns start hour of previous port-forwarding.
* **mercury-restart-tunnel**: if already started, kills port-forwarding, then restarts. if not, just starts.

## Installation:
```
$ git clone https://github.com/eckucukoglu/mercury-port-forwarding.git
$ cd mercury-port-forwarding
$ chmod +x install
$ sudo ./install
```
* Uninstall:

```
$ sudo ./install -u
```
