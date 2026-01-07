Ansible Role: QlikView Management
=========

An Ansible Role that allows for configuring QlikView using QMS APIs.

Requirements
------------

None.

Role Variables
--------------

```yaml
management_hostname: "{{ ansible_facts.hostname | default(ansible_host) }}"
qlikview_slk: AAAnfwebnfl...
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: qlik.qlikview.management
      qlikview_slk: AAAnfwebnfl...
```

License
-------

MIT

Author Information
------------------

This role was created by [Adam Haydon](https://github.com/ahaydon) of [Qlik Customer Success](https://github.com/QlikProfessionalServices)
