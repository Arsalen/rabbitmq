RabbitMQ
=========

Install RabbitMQ on Ubuntu 18.04 (Bionic).

Requirements
------------

Ubuntu Bionic.

Role Variables
--------------

Configures apt to install the most recent Erlang `22.x` version available in the repository and use packages for Ubuntu `18.04` (Bionic). More recent Ubuntu releases should also use this distribution name.

```yml
BIONIC_ERLANG_VERSION: 22.x
```

Dependencies
------------

These dependencies are available by default in Ubuntu 18.04 (Bionic).

- curl
- gnupg

Example Playbook
----------------

Example playbook.

```yml
- hosts:
    - server
  roles:
    - arsalen.rabbitmq
```

Example inventory.

```INI
[server]
123.456.78.9    ansible_user=user  ansible_ssh_pass=pass  ansible_become=true ansible_become_pass=pass
```

License
-------

BSD

Author Information
------------------

@arsalen ([github](https://github.com/Arsalen), [medium](https://medium.com/@arsalen.hagui), [linkedin](https://www.linkedin.com/in/arsalen-hagui-506979123/))