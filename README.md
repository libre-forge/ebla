# Ebla

This repository Ansible playbooks to be able to deploy libreforge
modules.

## roles

These are the available ansible roles:

- alexandria_boot: basic infraestructure to run `alexandria` module
- alexandria_release: playbook to deploy `alexandria` module
- viejnica_boot: basic infraestructure to run `viejnica` module
- common: playbook containing common tasks

All playbooks sensitive values have been replaced by placeholders. In
order to make them run you should provide your own `hosts` and
`extra-vars` files. Only then you could be able to execute the
playbook:

`ansible-playbook -i custom-host-file --extra-vars "@/path/to/extras-variables.yml" role_name.yml`
