# Join Linux Server to Active Directory 


## Description
This role performs all the steps need to join a Linux server to an Active Directory domain. I've only written tasks specifically for CentOS 7 and Ubuntu 16.04 LTS. Currently working on making one for Fedora 29. This role was originally intended as a step in a provisioning workflow using VMware vCenter, but can be adapted to join existing servers.

## Installed packages

### CentOS 7

- adcli
- realmd
- sssd
- sssd-tools
- ntp
- ntpdate
- samba-common
- samba-common-tools
- oddjob
- oddjob-mkhomedir
- python-pip

### Ubuntu 16.04 LTS

- realmd
- sssd
- sssd-tools
- adcli
- ntp
- ntpdate
- samba-common
- python-pip

## Variables

| Variable          | Description                                                                    |
| ----------------- | ------------------------------------------------------------------------------ |
| **adm_user**      | Username of domain admin or user allowed to join machines to the domain        |
| **adm_password**  | Password for the domain admin or privileged user                               |
| **prov_hostname** | If used to provision a server in vCenter, the hostname of the newly created VM |
| **prov_ip_addr**  | If used to provision a server in vCenter, the IP of the newly created VM       |

## Written By
David Hunter, 2018
