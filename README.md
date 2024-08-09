# Ansible Playbook Repository

Welcome to the Ansible Playbook Repository. This repository contains a collection of Ansible playbooks designed to automate various IT tasks, configuration management, and application deployment processes. Each playbook is organized by function and is intended to be reusable and easy to maintain.

## Table of Contents

- [Overview](#overview)
- [Directory Structure](#directory-structure)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Playbooks](#playbooks)
  - [Example Playbooks](#example-playbooks)
- [Contributing](#contributing)
- [Author](#author)

## Overview

This repository serves as a centralized location for all Ansible playbooks used within our organization. These playbooks are intended to be versatile, scalable, and easily customizable to meet the specific needs of various environments.

## Directory Structure

```
ansible-playbook-repo/
├── playbooks/
│   ├── playbook1.yml
│   ├── playbook2.yml
│   └── ...
├── roles/
│   ├── role1/
│   ├── role2/
│   └── ...
├── inventory/
│   ├── hosts.ini
│   └── ...
├── ansible.cfg
└── README.md

```

- **playbooks/: Contains the individual playbooks.
- **roles/: Stores reusable roles that can be referenced within playbooks.
- **inventory/: Hosts and groups definitions.
- **ansible.cfg: Ansible configuration file to define environment-specific settings.


## Requirements
Before running the playbooks, ensure that the following requirements are met:

- **Ansible: Version 2.9 or later.
- **Python: Version 3.6 or later.
- **Appropriate SSH keys or credentials for the target machines.
- **Inventory file configured for your environment.

## Getting Started
Clone the repository to your local machine:
```
git clone https://github.com/FatemehHABozorgi/Ansible-Playbook-Repo.git
cd ansible-playbook-repo
```
Configure your inventory file located in the inventory/ directory. Update the hosts.ini file with your server details.

## Usage
To run a playbook, use the following command:

```
ansible-playbook -i inventory/hosts.ini playbooks/playbook1.yml
```
You can specify additional options, such as tags or limiting the run to specific hosts:

```
ansible-playbook -i inventory/hosts.ini playbooks/playbook1.yml --tags "tag_name" --limit "host_group"
```

## Playbooks
Each playbook is designed to automate specific tasks. Below is a list of some of the key playbooks included in this repository:

### Example Playbooks
playbook1.yml: Description of what this playbook does.
playbook2.yml: Description of what this playbook does.
Each playbook is documented internally with comments and variable explanations to ensure ease of understanding and modification.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## Author
Created by Fatemeh Haji Agha Bozorgi.
