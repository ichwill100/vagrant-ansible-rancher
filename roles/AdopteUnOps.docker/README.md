# docker-ansible-role

Ansible role to install docker.
Only runs on ubuntu based machines

Role Variables
--------------

```
docker_package_name: docker-ce
docker_version: 17.06.2~ce-0~ubuntu
dockerpy_version: 1.8.0-*
docker_disks: /dev/sdb
docker_partitions: /dev/sdb1
docker_opts: "--log-opt max-size=50m --log-opt max-file=2"
use_docker_lvm: true
docker_repository_url: https://download.docker.com/linux/ubuntu/
docker_repository_category: edge
#this should be overrided only in case of downgrade of docker version
docker_force_version: no

#override this is you need use default ssl port
docker_registry_openssl_url: "{{ docker_registry }}"
```
License
-------

Apache License 2
