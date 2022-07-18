### What will this role do ?

The above bootstrap role will help you generate the DC/OS installation/configuration files on the various machines wherever you want to install DCOS.

#### Variable used in the role.

- path_bootstrap - This path stores the dcos configuration files .

- dcos_download_url - This specifies the url of the dcos_generate_config.sh file.

**Vars for DCOS enterprise**

The below variable is defined for enterprise DCOS configuration.

- enterprise_dcos: false

- security: permissive

**Vars for registry**

The below is for enabling registry to store files if you want to.

- registry: false

- enable_docker_gc: true

### How to run the playbook .

To run the playbook follow the below command:-

`ansible-playbook -i <your inventory file> playbook.yml`

**Note**:-  If you are running on your local system then you don't need to pass inventory file. Justy use localhost in hosts of playbook. 