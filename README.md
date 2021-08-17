# ansible-playbooks
Deploy SysAdmin Tasks

## Execute task

To deploy ansible playbooks you need to have groups of hosts in your /etc/ansible/hosts and the pass a target parameter with the group name.
Examples:

```bash
ansible-playbook [./ansible-playbooks/debian-get-basic-info.yml] -e target=my_group
```
