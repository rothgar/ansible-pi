ansible-pi
==========

Ansible playbook for setting up a raspi

### Usage

Run with

```
ansible-playbook -i inventory main.yml
```

If you only want to run on a single machine you can add `-e target=pi`. Default value is all

If you've never connected to a pi before you should disable host key checking with

```
ANSIBLE_HOST_KEY_CHECKING=False
```

If you only want to run one part of the playbook you can use tags

 * init
 * common
 * docker

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
- [x] split into separate roles
