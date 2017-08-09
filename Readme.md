About
-----

Ansible role for installing and using nfs as server and mount shares as client

Requirements
------------

...

Role Variables
--------------

Variables with examples:

```yml
# name of the nfs service running on the host. usually 'nfs'
nfs_service_name: nfs

##
```


Example Usage
-------------

```yml
roles:
  - nfs
vars:

```

Acknowledgements
----------------

thanks to
* [debops/ansible-nfs](https://github.com/debops/ansible-nfs)
* [openmicroscopy/ansible-role-nfs-mount](https://github.com/openmicroscopy/ansible-role-nfs-mount)


See also
--------

...

License
-------

MIT
