Ansible role for Graylog
=========

Requirements
------------

This role need Ansible 2.1. It's also supposed that
you are using the merge behaviour for variables (please, see about
[hash_behaviour=merge](http://docs.ansible.com/ansible/intro_configuration.html#hash-behaviour)
for details). Tested on Centos 6.5/7 and Debian 7/8

Dependencies
------------

1. Elasticsearch 2.x

2. MongoDB

3. Logstah (optional)

4. [Filebeat (optional)](https://github.com/fastpoke/ansible-filebeat)

Role Variables
--------------
Default config variables are described in */graylog/defaults/main.yml*.
If you need an extended configuration you can specify it in the variables for each environment in section *graylog.options*. You can insert any parameters described in official graylog [documentation](http://docs.graylog.org/en/2.1/)

Example Playbook
----------------
An example of how to use filebeat role:

    - hosts: all
      roles:
        - role: filebeat

License
-------

Apache-2.0


