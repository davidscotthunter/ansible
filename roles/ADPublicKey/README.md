# Active Directory SSH Public Key

## Description

This role configures authentication of Active Directory users by ssh public keys provided that it has been configured on 1) the domain controller via a procedure such as:

[LasLabs: Storing SSH keys in Active Directory for easy deployment](https://blog.laslabs.com/2016/08/storing-ssh-keys-in-active-directory/)

and 2) the correct configuration items are in your sssd.conf file.  If the server has been joined using the ActiveDirectoryJoin role, this is already configured.

## Written By
David Hunter, 2018


