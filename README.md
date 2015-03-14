ansible-pi
==========

Ansible playbook for setting up a raspi

Goals
=====

 * SSH tunnel
 * IRC bouncer (ZNC)
 * Cron jobs (StackStorm?)
 * WOL server
 * WeMo Web interface
 * DynDNS

### Usage

Add your own hosts file or run locally with

`ansible-playbook -i hosts.template -K pi.yml -e host=localhost`

The `-e host=` option needs to specify a host that is in your inventory file.
If you exclude the host variable the playbook will default to localhost.

