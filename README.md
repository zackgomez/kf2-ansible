An ansible script to set up a kf2 server with webadmin for further configuration

1/ Install the dependent roles: `ansible-galaxy install -r requirements.yml` (you might need sudo to install Ansible roles)
2/ copy `group_vars/all.yml.dist` to `group_vars/all.yml`
3/ edit `group_vars/all.yml` with appropriate values
4/ add machines to inventory file (one ip per line)
5/ run `ansible-playbook -i inventory kf2.yml`
6/ wait for server to run (you can use `docker ps` and `docker logs -f kf2server` on the target machines to watch progress
7/ webadmin should be running on ip:8080, username admin, use password from all.yml file
