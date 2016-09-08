Apigee Setup OS Minimum
=========

This roles setups the minimum operating system packages and configs that would allow OPDK to function properly. This is
a bare bones setup that can be considered a starting point but by no means the full OS setup. 

Requirements
------------

The installation of Apigee OPDK requires root access as does the installation of the system updates that are the focus 
of this role. Credentials must also be supplied to override the empty placeholders provided here. It is recommended that 
credentials be consolidated into a single credentials.yml file that can be stored separately. It is assumed that files 
containing credentials are stored in the ~/.apigee folder. 


Role Variables
--------------

Defaults for internal environment OPDK setup settings

    apigee_continue_on_warning: y

Default value to limit swap file use

    vm_swappiness: 60

Default epel repo for EL 6

    epel_ol6: https://dl.fedoraproject.org/pub/epel/epel-release-latest-6.noarch.rpm

Default epel repo for EL 7

    epel_rhel7: https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm

Dependencies
------------

No dependencies

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache License Version 2.0, January 2004

Author Information
------------------

Carlos Frias