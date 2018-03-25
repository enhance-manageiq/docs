## Embedded Ansible using AWX

### Background

In ManageIQ Fine release, it is configured to use [Ansible Tower](https://www.ansible.com/products/tower) for Embedded Ansible role. Integrating Ansible Tower in ManageIQ requires a tower license.

| Info | Procedure to setup Embedded Ansible in ManageIQ Fine version is described in [Setup Embedded Ansible](http://talk.manageiq.org/t/howto-setup-embedded-ansible/2291) |
|------|:------|

In Gaprindashvili release of ManageIQ, Ansible Tower is replaced by AWX for implementation of Embedded Ansible. [AWX](https://github.com/ansible/awx) is open source project around the Ansible Tower codebase. Unlike Ansible Tower, AWX doesn't requires license to be added for enabling Embedded Ansible in ManageIQ.

### AWX inside ManageIQ Appliance

AWX is deployed as group of containers inside ManageIQ appliance. EVM manage awx containers using the `docker-api` gem. When Embedded Ansible role is enabled on an appliance, it pulls latest awx docker images and run the containers.

To enlist docker images, type `docker images` in the terminal of ManageIQ appliance.

```
[root@localhost ~]# docker images
REPOSITORY                   TAG                 IMAGE ID            CREATED             SIZE
docker.io/ansible/awx_task   latest              e45b49c04679        4 days ago          1.017 GB
docker.io/ansible/awx_web    latest              2340b2955aa4        4 days ago          989.5 MB
docker.io/memcached          alpine              5c28baaba1e0        13 days ago         7.871 MB
docker.io/rabbitmq           3                   02c3edbcf3d1        3 weeks ago         126.9 MB
```

These four docker images are necessary to start awx properly.
AWX docker containers are linked together. To view the running containers, use `docker ps` command:

```
[root@localhost ~]# docker ps
CONTAINER ID        IMAGE                     COMMAND                  CREATED             STATUS              PORTS                                NAMES
88542be75c63        ansible/awx_task:latest   "/tini -- /bin/sh -c "   3 hours ago         Up 3 hours          8052/tcp                             awx_task
8cfc034ebffb        ansible/awx_web:latest    "/tini -- /bin/sh -c "   3 hours ago         Up 3 hours          0.0.0.0:54321->8052/tcp              awx_web
221989ad1c44        memcached:alpine          "docker-entrypoint.sh"   3 hours ago         Up 3 hours          11211/tcp                            memcached
0c0556dc8277        rabbitmq:3                "docker-entrypoint.sh"   3 hours ago         Up 3 hours          4369/tcp, 5671-5672/tcp, 25672/tcp   rabbitmq

```

| Note | If `docker ps` command doesn't display these containers then check the status of 'EmbeddedAnsibleWorker' using `cd vmdb; rake evm:status`. Make sure that its status is started.  |
|------|:------|

#### AWX Containers Log

After the containers are started, it is able to see their logs for monitoring awx progress.

To display logs in terminal, type command as follow:

```
# Tail the awx_task log
[root@localhost ~]# docker logs -f awx_task

```

#### Access AWX Bash

Sometimes, it is need to access bash for the containers like to check status of ansible job. To access the bash of awx_task, run `docker exec -it <container id> /bin/bash` command.

```
[root@localhost ~]# docker exec -it 88542be75c63 /bin/bash
[root@awx awx]# ls
beat.db      projects  supervisord.log	venv
favicon.ico  public    supervisord.pid	wsgi.py
[root@awx awx]#

```

Path `/var/lib/awx/job_status/` in container stores the status of tower job.
