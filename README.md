Simple provisioning for server to use as teamspeak server and web server.
This playbook:
1. Creates two users.
2. Enable systemd (systemctl --user) and journal (journalctl --user-unit) for them.
3. Installs ts3 server for user teamspeak

To run (require python2.7 and pip):
1. Fill inventory with server host
2. Fill passwords ids etc. in playbook (server.yml)
3. ```make install``` to install ansible
4. ```make provision``` to run ansible

After reboot users should be able to use systemd.