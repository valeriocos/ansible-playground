# Ansible-playground

This repo contains some toy Ansible playbooks

# Requirements

- ansible
```
$ python3 -m venv /home/ansible-env
$ source /home/ansible-env/bin/activate
$ (ansible-env) pip install ansible
```

# Execution

```
$ (ansible-env) ansible-playbook
--connection=local
--inventory 127.0.0.1
--limit 127.0.0.1
playbook-hello.yml
-i ansible_hosts
--ask-become-pass (needed if a task requires to install apt packages, playbook-git)
```