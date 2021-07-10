Role Name
=========

Role to mount Common Internet File System. 

Requirements
------------

This role was created for Debian based linux distributions.

Role Variables
--------------

Required role variables:

```yaml
# CIFS server host and share
cifs_location: "//host/share"

# The credentials of the user with permission to access the share
cifs_username: username
cifs_password: password

```

Optional variables:

```yaml
# Mountpath
cifs_mountpath: "/var/lib/longhorn"
```


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: cifs
      roles:
         - ansible-role-cifs-mount

License
-------

GNU GENERAL PUBLIC LICENSE VERSION 3

Author Information
------------------
[blog.retter.jetzt](https://blog.retter.jetzt)

