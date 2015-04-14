# Ansible role to install Unicorn

[![Build Status](https://img.shields.io/circleci/project/crushlovely/ansible-unicorn-upstart.svg?style=flat)](https://img.shields.io/circleci/project/crushlovely/ansible-unicorn-upstart)
[![Current Version](http://img.shields.io/github/release/crushlovely/ansible-unicorn-upstart.svg?style=flat)](https://galaxy.ansible.com/list#/roles/1180)

This Ansible role installs/updates and configures Unicorn.  It also copies a working Upstart script.

## Installation

``` bash
$ ansible-galaxy install crushlovely.unicorn-upstart,v1.0.0
```

## Variables

``` yaml
app_name: test
app_path: /home/ubuntu/test
app:
  process_name: {{ app_name }}
```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
- hosts: localhost
  roles:
    - crushlovely.unicorn-upstart
```

## Dependencies

None

## License

MIT