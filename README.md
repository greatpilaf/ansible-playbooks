# ansible-playbooks
Deploy SysAdmin Tasks

## Execute task

To deploy ansible playbooks you need to have groups of hosts in your /etc/ansible/hosts and the pass a target parameter with the group name.
Examples:

```bash
ansible-playbook [ansible-playbook.yml] -e target=my_group
```
## Playbooks:

### 1. linux-report.yml

This playbook will create a report of a Linux (Debian or RedHat).

What kind of information can you have with this playbook?

1. Hostname
2. OS Name
3. OS Version
4. Domain
5. Main IP
6. Default Gateway
7. Service TAG (if apply)
8. System Manufacturer (if apply)
9. Used Space on Main dirs
10. Server Uptime
11. RAM Summary
12. Miliseconds to gateway
13. Fail2ban Summary (if apply)
14. Open ports and listen (if apply)
15. DISKS Summary (if apply)

#### How execute
```bash
ansible-playbook linux-report.yml -e target=my_group -K -e lang=[español-english]
```


