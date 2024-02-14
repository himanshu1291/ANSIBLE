nfs-client
=========
This role will help you to configure nfs-clients that can access shared directory by nfs-server

Requirements
------------
OS should be rpm based such as RHEL centOS Fedora ! 

Role Variables
--------------
"{{ access_dir }" is the variable that saves the value of directory through which shared directory can be accessed on nfs-client
"{{ ipaddress_nfs_server }}" will take the IP address of nfs-server so that it can be used to mount on nfs-client
"{{ shared_dir }} takes the absolute path of the shared directory [ by nfs-server ]
NOTE: value of these variables can be define in roles/nfs-client/vars/main.yml



Example Playbook
----------------


    - name: Configuring nfs-client 
      hosts: nfs-client
      roles:
         - nfs-client




