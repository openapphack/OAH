**Layout**

 Must be a GIT repo accesible to oah-shell

 Must be a valid Ansible Role

**Naming Convention** :

Must follow the naming convention of ***ansible-role-oah-XXXX*** where XXXX is the oah community accepted name that clearly mentions the purpose of the roles.

**Must Have files** : 

Each oah ansible role must have the following Task files in the tasks folder of the ansible role

- main.yml
- oah-install.yml
- oah-remove.yml
- oah-reset.yml
- oah-update.yml 
- oah-validate.yml

OAH task yml files should have tasks to safely install, update, reset , validate or remove the all changes done by the role. 

Each OAH role will have a in-built Task to validate (and determine) if the role has been successfully installed.

EACH OAH Roles must follow the best practices as mentioned(http://docs.ansible.com/ansible/playbooks_best_practices.html)

**OAH Ansible Role  Variables**

All OAH Ansible Variables will begin with a oah_

oah_command : Is used to determine the operation mode of a role. 

oah_command param can have the following values => **install** , **remove** , **reset** , **update** and **validate** )

oah_command will default to update , it can have values install,remove, reset, update and validate. (i.e If OAH_COMMAND env variable is not set by the oah-scripts and if the environment playbooks are not set by the oah_command variable, main.yml will include oah_update.yml or oah_install.yml if the role has not be installed yet.)

