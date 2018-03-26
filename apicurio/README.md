# Apicurio 

This quickstart is an [openshift-applier inventory](https://github.com/redhat-cop/openshift-applier) to deploy [Apicurio](https://www.apicur.io/). It's derived from [Mike Hepburn's work](https://github.com/eformat/openshift-apicurio).

## Prerequisites

* Either [Docker CE](https://www.docker.com/community-edition#/download) or [Ansible](http://docs.ansible.com/ansible/latest/intro_installation.html)
* [OpenShift CLI Tools](https://docs.openshift.com/container-platform/3.7/cli_reference/get_started_cli.html)
* Access to the OpenShift cluster with privileges to create Projects

## Usage With Docker

1. Log into OpenShift
2. Make sure the docker daemon is running on your host
3. ```[apicurio]$ ./run.sh```

## Usage Without Docker

1. Log into the relevant OpenShift cluster
2. ```[apicurio]$ ansible-galaxy install -r requirements.yml --roles-path=roles```
3. ```[apicurio]$ ansible-playbook roles/casl-ansible/playbooks/openshift-cluster-seed.yml -i inventory/```