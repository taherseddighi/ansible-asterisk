# Asterisk Installation Playbook

This repository contains an Ansible playbook to automate the installation of Asterisk on remote hosts.

## Prerequisites

Before running the playbook, ensure you have the following:

- Ansible installed on your control machine.
- SSH access to target hosts with appropriate privileges.
- An inventory file defining the target hosts.

## Creating an Inventory File

Create an inventory file (e.g., `inventory.yml`) with the following structure:

```
[asterisk_hosts]
server1.example.com
server2.example.com
```

Modify the inventory file according to your environment.

## Running the Playbook

To install Asterisk on the specified hosts, run the following command:

```
ansible-playbook -i inventory.yml install-asterisk20.yml
```

This will execute the installation process on all hosts listed in the inventory.

## Notes

- Ensure that your Ansible configuration allows SSH connections to the target hosts.
- You may need to specify a user with `-u <username>` and use `--ask-become-pass` if sudo access is required.


## Contributions

Feel free to open issues or submit pull requests to improve this playbook.

