# rh1-lab19-satellite


The Playbooks in each of the directories are built to run with the modules in [rh1-lab19-satellite](https://github.com/RedHatQuickCourses/rh1-lab19-satellite).

These require the redhat.satellite Ansible Collection to run - This may be installed either from Automation Hub, or from the Satellite Repositories.

ansible-galaxy collection install redhat.satellite

You can also include it in a requirements.yml file and install it with ansible-galaxy collection install -r requirements.yml, using the format:

collections:
  - name: redhat.satellite


The init_scripts/playbook.yml is meant to run when the lab is provisioned and should set up all of the required variables to continue running the additional playbooks found in each module.

Required Variables:

bastion_public_hostname  
bastion_ssh_password  
bastion_ssh_user_name  
cloud_provider  
guid  
showroom_host  
showroom_primary_view_url  
ssh_command  
ssh_password  
ssh_username  
subdomain  
subdomain_internal  
targethost  
workshop_satellite_url  
workshop_satellite_user_name  
workshop_satellite_user_password  

