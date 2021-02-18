DLNA Ansible role
==================

Role to manage DLNA.

Requirements
------------

No requirements

Role Variables
--------------

`dlna__install:` For install only (default: False)
`dlna__configure:` For configuration  (default: False)
`dlna__name:` Human readable share name (no Default)
`dlna__inotify:` Use inotify to check libraries changes (Default: "no")
`dlna__shares:` List of library shares (default: [])


Dependencies
------------

None

Example Playbooks
-----------------

Play with:

```
- hosts: all
  name: Setup DLNA server
  roles:
    - role: dlna
```

With vars like:

```
dlna__shares:
  - path: /var/lib/music
    type: A
  - path: /var/lib/film
    type: V
```

License
-------

GPLv3

Author Information
------------------

François TOURDE

