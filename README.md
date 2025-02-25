ansible-mount-device
=========

Mount the given block device

Requirements
------------

None

Role Variables
--------------

`devices`: a list of objects, describing which device should be mounted, and how (see below for an example) 

Dependencies
------------

None

Example Playbook
----------------

```yaml
- role: mount_device
  devices:
    - what: /dev/vdb
      where: "/somewhere"
      fstype: ext4
      opts:
        - noatime
      state: mounted
```

License
-------

BSD

Author Information
------------------

corvus-migratorius@proton.me
