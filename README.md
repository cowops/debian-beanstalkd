Debian-Beanstalk
================

Beanstalk is a simple, fast work queue.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

beanstalkd_listen_addr: "0.0.0.0"
beanstalkd_listen_port: "11300"
beanstalkd_start: "yes" (allows beanstalkd autostart)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: loranger.debian-beanstalkd, beanstalkd_listen_addr: "0.0.0.0", beanstalkd_listen_port: "11300", beanstalkd_start: "yes" }

Tasks
-----

  - Install [Beanstalk](http://kr.github.io/beanstalkd/) server

License
-------

BSD