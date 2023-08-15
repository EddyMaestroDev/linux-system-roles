# Ansible Collection - Linux System Roles

This is unified Ansible collection to centrally manage many Linux system settings, for open(SUSE), Red Hat/ CentOS and Debian based Distris on Bare-Metal, Vmware vSphere, IBM PowerVM or Cloud Managed Installation.

This role is suitable for system rollout, manage existing systems with ansible to verify some Settings and/or to change them.

The following settings are managed with it:
- Subscription Management (Linux SUSE Enterprise and Red Hat Enterprise Distributions)
- local Users, Pre-Shared-keys and sudoers
- Set Plattform specific settings and install/Update latest Hypervisor Tools (vSphere, PowerVM, Cloud, Bare-Metal etc.)
    - for Example: I/O Scheduler, Kernel oder mutipath Settings
- Manage SSL Certificates (PKI)
- NTP Client
- Network Settings
    - DNS Servers
    - /etc/hosts entries
    - Firewall
    - SELinux/ AppArmor
- Microsoft Actice Direcory Management
- Manage other Core Services, for example Postfix, SSHD etc.
- System Hardening with OpenSCAP und CIS Profile

Requirements
------------

Basic installed Linux System with Ansible Package, existing ansible User and exchanged PSK for the ansible User.

Installation
------------

ansible-galaxy install EddyH85.linux_system_mgmt

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache 2.0

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).


