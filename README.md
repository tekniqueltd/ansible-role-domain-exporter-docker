Role Name
=========

Ansible role that deploys a domain-exporter which receives information and exports them as prometheus metrics to http://localhost:9222/probe

Supported Operating Systems
---------------------------

- Debian 9+
- Ubuntu 16.04+ (untested)

Requirements
------------

- Ansible 2.4+ (on execution host)
- Docker 17+ (on remote host)

Role Variables
--------------

See `./defaults/main.yml` for configurable variables and their defaults

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - name: Example play with some optional vars set
      hosts: all
      roles:
        - { role: domain-exporter-docker
          }

Add as a submodule to your playbook repo

    git submodule add  https://github.com/tekniqueltd/ansible-role-domain-exporter-docker.git roles/domain-exporter-docker
