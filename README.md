# Development Environment Setup with Ansible

This repository contains Ansible playbooks and configuration files to automate the setup of my development environment. It installs relevant packages and applications to ensure a consistent and efficient development setup across different machines.

## Prerequisites

Before running the playbooks, ensure you have the following installed on your system:

- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) (version 2.16 or later)
- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
   ```

2. Install required Ansible roles:

    ```sh
    ansible-galaxy install -r requirements.yml
    ```

## Usage

To set up the development environment, run the following command

```sh
ansible-playbook main.yml --ask-become-pass
```

This command will execute the setup.yml playbook, prompting you for your sudo password to install the necessary packages and applications.

## TODO
- [] Clone and setup dotfiles
- [] Make this work for MacOS