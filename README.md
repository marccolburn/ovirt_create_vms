oVirt Create VMs
=========

Create VMs for Network Auto Lab in oVirt

Requirements
------------


Role Variables
--------------
virtual_machines:
* name: Name of VM
* template: Template to create VM off of
* cluster: oVirt cluster VM should be created on
* nics: List of NICs to attach
  * name: Name of NIC
  * interface: Interface type [e1000,virtio,etc.]
  * profile_name: vNIC profile to attach

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: ovirthost
      roles:
         - { role: ovirt_create_vms }

License
-------

BSD

Author Information
------------------

Marc Colburn Red Hat
