# Ansible
Ansible student assignment

Web application is deployed on DOCKER environment. For image was used docker image- mmumshad/ubuntu-ssh-enabled. Hosts ip address: 172.17.0.2, 172.17.0.3, 172.17.0.4, 172.17.0.5
It used two groups of hosts- [hosts] for web app deploy, [spare_host] for experiments and check deployments.
inventory file is encrypted by Ansible vault. Password is stored in vault_pass.txt
All tasks are splited to roles- deploy_python for deploying depencies, deploy_db for deploying mysql db, deploy_web for deploy flask and web app.
At the end of playbook ansible check that all tasks is completed, and send report by mail
