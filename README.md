volkula.docker_bundle
=========

Install docker and docker-compose

Requirements
------------

- python3

Role Variables
--------------

```yml
vars:
    install_by: curl - Install by curl get.docker.com
    install_by: pip  - Install by pip3
    install_by: repo - Install by Docker repo
    compose_version: - auto-detect version by github tag
```

Dependencies
------------

collections:
- name: community.general

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- name: DockerCompose
  hosts: docker
  become: true
  gather_facts: true
  vars:
    install_by: "pip"
  roles:
    - volkula.docker_bundle
```

License
-------

BSD

Author Information
------------------

Made by Volkula (https://github.com/Volkula) 2022
