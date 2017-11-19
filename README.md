Ansible Role: Docker Secrets
=========

Manage sensitive data with Docker secrets [Docs](https://docs.docker.com/engine/swarm/secrets/#read-more-about-docker-secret-commands)

Requirements
------------

Swarm Mode should be enabled on target.

Role Variables
--------------

List of secrets:

```
secrets:
  hello: "world"
```

Dependencies
------------

None.

Example Playbook
----------------


    $ cat inventory
    [servers]
    172.10.10.1

    $ cat playbook.yml
    - name: "Setup Docker Secrets"
      hosts: servers
      roles:
        - { role: mlabouardy.docker-secrets }

License
-------

MIT

Author Information
------------------

Mohamed Labouardy ([@mlabouardy](https://twitter.com/mlabouardy))
