Ansible Role: QlikView setup
=========

An Ansible Role that installs QlikView Enterprise.

Requirements
------------

None.

Role Variables
--------------

```yaml
setup_path: '{{ ansible_env.HOME }}\Downloads\Qlik_Sense_setup.exe'
setup_username: '{{ ansible_netbios_name }}\qvservice'
setup_password: "Qlik1234"
setup_features: [all]
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: qvservers
  roles:
    - role: qlik.qlikview.setup
      setup_path: '{{ ansible_env.HOME }}\Downloads\QlikViewServer_x64Setup.exe'
      setup_username: '{{ ansible_netbios_name }}\qvservice'
      setup_password: "Qlik1234"
```

License
-------

MIT

Author Information
------------------

This role was created by [Adam Haydon](https://github.com/ahaydon) of [Qlik Customer Success](https://github.com/QlikProfessionalServices)
