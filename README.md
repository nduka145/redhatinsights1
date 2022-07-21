Role Name
=========
Ansible-insights role installs and register Redhat insights

Requirements
------------
The ansible insights role can only run on redhat servers

Role Variables
--------------
Important variables are defined in defualts/main.yml fils as;

  insights_supported_actions:

    - install    # Installs Redhat insight Client

    - uninstall  # Unstalls Redhat insight client

    - reinstall  # reinstalls insights


  insights_target_action: install


Playbook Usage 
------------

# Playbook can be run as;

  To install - ansible-playbook insight.yml --extra-vars "insights_target_action=install"

  To uninstall - ansible-playbook insight.yml --extra-vars "insights_target_action=uninstall"

  To reinstall - ansible-playbook insight.yml --extra-vars "insights_target_action=reinstall"
   
