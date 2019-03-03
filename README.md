swiss-army
==========

[![License: BSD 3-Clause License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![Build Status](https://travis-ci.org/jwflory/swiss-army.svg?branch=master)](https://travis-ci.org/jwflory/swiss-army)

Ansible-driven configuration management for maintaining a preferred environment (base system and app configurations)

[![Ansible-driven swiss army knife](https://openclipart.org/image/300px/svg_to_png/98191/swiss-knife.png)](https://openclipart.org/detail/98191/swiss-knife)


## About

swiss-army is my "swiss army knife" to set up and manage my preferred Linux environment.
It is a set of Ansible playbooks and roles.
Roles are split into two categories:

* `system`: base system configuration (e.g. package installation)
* `apps`: specific app installation and configuration (e.g. dotfile management)

For a fully automated setup, two environments are supported: **Fedora** and **CentOS/RHEL**.


## How to use

See [`docs/how-to-use.adoc`](https://github.com/jwflory/swiss-army/blob/master/docs/how-to-use.adoc "How to use jwflory/swiss-army").

```
    ansible-galaxy -K install -r requirements.yaml
    ansible-playbook -K playbooks/fedora-workstation.yml
```
