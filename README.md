Role Name
=========

Take a fresh deployed server from AWS or Digital Ocean and deliver it with everything it needs to be a secure, easy to use simple server.  Servers will be deployed via Tugboat for Digital Ocean and AWS will use Web or cli.

  - Goal:
    - Apply all updates via YUM or Apt
    - Apply sane security setup
    - Create a list of users
    - Each user should have:
      - SSH Keys loaded
      - Shell configured
      - Aliases ready
      - Sudo access

Requirements
------------

  - Server is running
  - Server has a public facing IP
  - SSH is enabled

Role Variables
--------------

users_ssh_key_pass = password for the ssh key created on the delivered server
delivered_users = users to create on the system that will have sudo


Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

GNU

Author Information
------------------

Chris Livermore

[@e30chris](https://twitter.com/e30chris)

[Sandors Systems Scribbles](http://sandorsscribbl.es/)
