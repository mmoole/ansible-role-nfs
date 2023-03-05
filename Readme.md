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
nfs_service_name: nfs-server

# defaults for nfs-mounts:
# List of NFS shares
nfs_share_mounts: []

# example:
#nfs_share_mounts:
#   - path: /mnt/remote
#     location: nfs.example.org:/data
#   - path: /mnt/readonly
#     location: nfs.example.org:/read-only
#     opts: "{{ nfs_mount_opts }},ro"

# Default NFS4 mount options
nfs_mount_opts: rsize=8192,wsize=8192,timeo=14,intr

```


Example Usage
-------------

```yml
roles:
  - nfs
vars:
nfs_share_mounts:
   - path: /mnt/remote
     location: nfs.example.org:/data
   - path: /mnt/readonly
     location: nfs.example.org:/read-only
     opts: "{{ nfs_mount_opts }},ro"

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
