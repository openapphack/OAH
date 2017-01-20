**Layout**

OAH CLUSTER will be a git repository

Must have a provisioning and testing folder


**Naming Convention** :

OAH CLUSTER git repository will have the following naming convention OAH-XXXX-CLUSTER . where XXXX is the VM Type Name that uniquely identified the purpose of the VM


**Must Have files** : 

Must have an invertory file and each group in the inventory file can have one or more vm

OAH CLUSTER provisioning folder must have subfolder for each vm in the cluster
 
Each vm in the cluster will have playbook.yml as well as install.yml, reset.yml & remove.yml 
Must have a requirements.yml in the each vm folder


OAH CLUSTER must have VagrantFile,in vagrant folder ,  
DockerFile  in docker folder and a raw install.sh in top level ove-cluster root folder
 
