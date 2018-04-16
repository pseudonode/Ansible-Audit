It has proven useful for large network audits where dozens of commands in dozens or potentially hundreds of devices need to be retrieved as part of information gathering activities within large networks.

Each IOS command will generate one file.
Example: the play called "Show Running Configuration" will create a file called [hostname of device]_show_run.txt with the relevant output of a "show running-config" command. If the Ansible invnetory file has 20 hosts inside then 20 files will be created

If a single file is required instead of one file per command then the ansible assemble module can be utilised for such purpose with the relevant play configured for such effect in the end of the playbook.

This playbook was created with Cisco IOS in mind but can easily be repurposed to use any platform with the relevant core modules (nxos_command, eos_command, etc.)

This PB was tested in Ansible 2.2, 2.3 and 2.4
