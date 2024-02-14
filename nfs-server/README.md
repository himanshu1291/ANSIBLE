nfs-server
=========

This roles deals in basic configuration of nfs-server

Requirements
------------
supports on Centos RHEL Fedora OS.

This role includes firewall configuration. If you are using IPtables or other security tool then the firewall configuration should be commented in playbook.


Role Variables
--------------
used variable is "{{ shared_dir }}". Value of this variable is defined under roles/nfs/vars/main.yml 


Example Playbook
----------------

example of how to use your role:

    - name: Configuration of nfs-server 
      hosts: nfs-iserver.example.com
      roles:
         - nfs-server  


Author Informatio
