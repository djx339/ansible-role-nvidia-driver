Ansible Role: Nvidia Driver
=========

Install Nivida driver on Linux System.

Requirements
------------

None.

Role Variables
--------------

`nvidia_driver_version`: The version of nvidia driver. (eg. latest, 384) (Default: latest)

`nvidia_driver_use_ppa`: Using `ppa:graphics-drivers/ppa` or not. (Default: False)

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: all
  become: yes
  vars:
    nvidia_driver_version: latest
    nvidia_driver_use_ppa: False
  roles:
    - { role: djx339.nvidia-driver }
```

License
-------

BSD

Author Information
------------------

This role was created by [Daniel D](https://github.com/djx339).
