Ansible Sentry
=========

A easy installation for sentry service

Requirements
------------

+ python 2.7
+ docker CE 
+ pip
+ centos  

Please add the user in the controlled matchine to the "docker" group, otherwise postgres, redis needs to be installed by sudo user

#Add docker group
`sudo groupadd docker`

#Add user to docker group
`sudo usermod -aG docker $USER`

#REMIND to start docker daemon
`sudo systemctl statrt docker`

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

Pleaase make sure docker is installed on your target remote machine
[Install docker ce on Cent-OS](https://docs.docker.com/engine/installation/linux/docker-ce/centos/#install-using-the-repository)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
