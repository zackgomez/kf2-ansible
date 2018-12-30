An ansible script to set up a kf2 server with webadmin for further configuration

copy `group_vars/all.yml.dist` to `group_vars/all.yml` and edit file

add machines to inventory file (one ip per line)

run

```
ansible-playbook -i inventory kf2.yml
```
