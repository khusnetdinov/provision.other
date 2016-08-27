# Provision.zsh
[![Galaxy](https://img.shields.io/badge/galaxy-provision.zsh-blue.svg?style=flat-square)](https://galaxy.ansible.com/khusnetdinov/provision.zsh/)

This is ansible receipt for installing zsh user for linux (Ubuntu). It also is used in other [provision receipt](https://github.com/khusnetdinov/provisioner) for prepare production enviroment on server.

#### Variables

```yaml
provision_user: deploy             # The name of deploy user
```

#### Usage

Add `provision.zsh` to your roles and set vars in your vars file or playbook file.

requirements file:

```yaml
- src: "https://github.com/areceipt/provision.zsh"
  name:  zsh
```

  vars_file:

```yaml
provision_user: deploy
```

playbook:

```yaml
- hosts: all
  roles:
    - role: zsh
``````
