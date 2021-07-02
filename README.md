PBIS-Open
=========

Its role is designed to install and configure PBIS-Open with a Microsoft Active Directory

Compliance
----------
|Redhat|Centos|Debian|Ubuntu 18.04|Ubuntu 20.04|
|-|-|-|-|-|
|Unknown|Unknown|Unknown|Unknown|Unknown|

Requirements
------------

* A Microsoft active directory server
* A user with domain admin on the AD

Role Variables
--------------

  domain_fqdn: 
  Choose  the FQDN for the AD Default: office.contoso.com
  
  domain_netbios: 
  Choose netbios name for the AD. DEFAULT:CONTOSO
  
  domain_user: 
  Your domain username. Default: USERNAME
  
  domain_pass: 
  Your domain Password: Default: PASSWORD
  
  domain_admingroup: 
  The domain group for adminprivileges Default: unix_ux_admin

  domain_creategroups: True
  Automatically create groups for each servers (srv_$hostname_auth for login and srv_$hostname_sudo for root access)
  
Example Playbook
----------------

Please check site.yml
