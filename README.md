
# ansible-project-commands

**Automated Deployment of Jupiter Website on EC2 Instances**

**Author:** Christiana Bello

This repository contains an Ansible playbook that automates the deployment process of the Jupiter website on EC2 instances. It streamlines the setup and configuration of the Apache server and ensures the latest version of the website is deployed.

## Prerequisites
Before running this playbook, ensure the following prerequisites are met:

- Ansible is installed on the control node machine.
- EC2 instances are set up and accessible from the control node.
- SSH access is configured between the control node and EC2 instances.

## Playbook Overview
The playbook executes the following tasks:

1. **Update Packages:** Updates all packages on the EC2 instances to ensure they are up to date.
2. **Install Apache Server:** Installs the Apache HTTP server on the EC2 instances.
3. **Download Website Files:** Downloads the latest version of the Jupiter website from the GitHub repository.
4. **Extract Website Files:** Extracts the downloaded ZIP file containing the website files.
5. **Copy Website Files:** Copies the website files to the appropriate directory for hosting (/var/www/html/).
6. **Clean Up:** Removes the temporary ZIP file and directory used for extraction.
7. **Start Apache Server:** Starts the Apache HTTP server if it is not already running.

## Customization 
- Update the GitHub repository URL in the playbook to point to your own repository if needed.
- Adjust the directory paths and filenames according to your server configuration.



## Ansible Playbooks and Modules Resources
[Ansible Plabook](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_intro.html)
[Ansible Modules](https://docs.ansible.com/ansible/2.9/modules/list_of_all_modules.html)


