[![CircleCI](https://circleci.com/gh/orangesys/ansible-role-telegraf.svg?style=svg)](https://circleci.com/gh/orangesys/ansible-role-telegraf)
Orangesys telegraf
=========

An Ansible role to install, configure, and manage [Orangesys Telegraf](https://github.com/orangesys/telegraf), the plugin-driven server agent for reporting metrics into InfluxDB.


Requirements
------------

Prior knowledge/experience with Orangesys Saas and Telegraf is highly recommended.

Role Variables
--------------

The high-level variables are stored in the `defaults/main.yml` file. The most important ones being:

```
# Channel of Telegraf to install (currently only '1.3.2' is supported)
telegraf_agent_version: '1.3.2' or highly

```

Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars:
      orangesys_url: 'demo.i.orangesys.io'
      orangesys_jwt_token: 'jwt-token'
      roles:
         - { role: ansible-telegraf, tags: telegraf }

License
-------

MIT

Author Information
------------------

[Orangesys .Inc](https://orangesys.io)
