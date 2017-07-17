Role Name
=========

Install docker.

Requirements
------------

ubuntu 14.04 only for now.

Role Variables
--------------

TODO docker_version variable.

Dependencies
------------

none.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD, MIT

Author Information
------------------

https://github.com/chshawkn



How to create a role in ansible-galaxy like this
------------------
```sh
ansible-galaxy init <role-name>
mv <role-name> ansible-role-<role-name>
cd ansible-role-<role-name>
git init
# coding ...
git add .
git commit -m 'init commit'

git remote add origin git@github.com:<owner,org>/ansible-role-<role-name>.git
git push -u origin master

ansible-galaxy login --github-token ${GITHUB_INFRASTRUCTURE_CONF_GIT_TOKEN}
ansible-galaxy import <owner,org> ansible-role-<role-name>
```

see: https://docs.ansible.com/ansible/galaxy.html
