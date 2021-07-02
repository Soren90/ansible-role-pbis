PBIS-Open
=========

Its role is designed to install and configure PBIS-Open with a Microsoft Active Directory

Compliance
----------
|RHEL 8|Debian 10|Ubuntu 20.04|
|-|-|-|
|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|

Requirements
------------

* A Microsoft active directory server
* A user with domain admin on the AD

Role Variables
--------------

Choose  the FQDN for the AD Default: office.contoso.com
  
    domain_fqdn: office.contoso.com

Choose netbios name for the AD. Default: CONTOSO
  
    domain_netbios: CONTOSO

Your domain username. Default: USERNAME
  
    domain_user: ad-user

Your domain Password: Default: PASSWORD
  
    domain_pass: v3rys3cur3

The domain group for adminprivileges Default: unix_ux_admin
  
    domain_admingroup: unix_ux_admin

Automatically create groups for each servers (srv_$hostname_auth for login and srv_$hostname_sudo for root access) Default: True
  
    domain_creategroups: True

  
Example Playbook
----------------

Please check site.yml
