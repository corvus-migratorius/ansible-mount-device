Role Name
=========

Mount the given device

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

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

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
