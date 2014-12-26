Role: cns.awscli
========

This role installs and configures awscli for specific users

Requirements
------------

Nothing, it runs out of the box.

Role Variables
--------------

In the current version, you can specify the following variables:

| Name               | Default |                                                              |
|--------------------|---------|--------------------------------------------------------------|
| admin_users        |   ---   | List containing all users that require ansible environment.  |
| aws_access_key     |   ---   | AWS Access Key.  Required for $HOME/.aws/config (use vault)  |
| aws_secret_key     |   ---   | AWS Key Secret. Required for $HOME/.aws/config (use vault)   |
| aws_region         |   ---   | Default region for awscli. Required for $HOME/.aws/config    |


Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by Sam Morrison
https://www.twitter.com/samcns

Examples
--------

```yaml
---
- name: common role test
  hosts: all
  roles:
    - cns.ansible
```
