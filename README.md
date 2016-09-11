ansible-pi
==========

Ansible playbook for setting up a raspi

### Usage

Run with

`ansible-playbook -i inventory pi.yml`

If you only want to run on a single machine you can add `-e target=pi`. Default value is all

Goals
=====

 * Expand rootfs
 * Set hostname
 * Secure SSH
 * Change pi users password (random)
 * Install docker
 * Install basic packages

### ToDo

- [ ] init docker swarm
- [ ] run containers
