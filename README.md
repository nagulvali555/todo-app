# todo
- sample todo application deployment
- todo app repo: https://github.com/docker/getting-started.git

## AnsibleDeployment
Deploying the application using ansible

### Prerequisites
- create two vms one for mysql and one for application
- copy ansible vm ssh public ip to the newly created vms in ```~/ssh/.authorized_keys``` file
- check ssh connectivity for the two vms from ansible, make sure ansible able to ssh vms.

### Deployment
- clone the repository
- update inventory file with frontend vm ip and database vm ip
- run ```ansible-playbook deploy.yaml```