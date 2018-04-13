# Ansible-Audit

The purpose of this Ansible playbook is to connect to multiple devices and issue a series of commands and then copying the output of those commands to a .txt file

It has proven useful for large network audits where dozens of commands in dozens or potentially hundreds of devices need to be retrieved as part of information gathering activities.

If a single file is required instead of one file per command then the ansible assemble module can be utilised for such purpose.
