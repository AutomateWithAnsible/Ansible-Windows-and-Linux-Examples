Ansible Role Development
=========

Basic walkthrough of creating an Ansible role.

Requirements
------------

```Ansible```

Role Creation
--------------

Change into the directory where your Ansible Roles are stored and then following command to create a new role:

```ansible-galaxy role init <role_name>```

The Anatomy of a Role
------------

The following is the directory structure of a role:

    /defaults
    /files
    /handlers
    /meta
    /tasks
    /templates
    /tests
    /vars
    README.md

Each directory contains a file named main.yml except for files and templates.

How to run a Playbook
---------------------

## Linux Hosts
```ansible-playbook <playbook_name.yml>```

## Windows Hosts
```ansible-playbook -i ./Inventory/Windows-Hosts.yml ./playbooks/Windows.yml```

Playbooks to create
---------------------

1. Download file from URL
2. Archive a Directory
3. Unarchive a Directory
