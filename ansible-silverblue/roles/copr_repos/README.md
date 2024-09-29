copr_repos
================

This role adds [copr_repos](https://copr.fedorainfracloud.org/coprs/)
onto an rpm-ostree host such as Fedora Silverblue.

Requirements
------------

Modules used:

  * [ansible.builtin.get_url module](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/get_url_module.html)

Role Variables
--------------

These varables are set in the project's `group_vars/all` file. Make your edits there!

  * copr_repos: Add these repos.

Dependencies
------------

None

Example Adhoc Run
-----------------

`ansible-playbook -i hosts -l this_host -K roles/copr_repos/playbook.yml`

Example Playbook
----------------

    - hosts: all
      roles:
        - { role: copr_repos }

License
-------

BSD

Author Information
------------------

  * John Gardiner (john@b234r.net)
