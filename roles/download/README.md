Ansible Role: QlikView download
=========

An Ansible Role that downloads QlikView setup from GitHub.

Requirements
------------

None.

Role Variables
--------------

```yaml
release_name: September 2025 SR1
download_path: "{{ lookup('ansible.builtin.env', 'HOME') }}/Downloads"
setup_path: "{{ download_path }}/{{ release_name }}/QlikViewServer_x64Setup.exe"
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: qlik.qlikview.download
      release_name: September 2025 SR1
```

License
-------

MIT

Author Information
------------------

This role was created by [Adam Haydon](https://github.com/ahaydon) of [Qlik Customer Success](https://github.com/QlikProfessionalServices)
