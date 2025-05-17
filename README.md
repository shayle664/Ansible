# 🧪 Ansible Summary Practice

This project demonstrates a simple Ansible playbook used to automate script distribution and execution across multiple nodes.

## 📁 Project Structure
.
├── ansible.cfg # Ansible configuration pointing to the inventory file
├── hello.sh # Shell script to be copied and executed on all nodes
├── hosts.ini # Inventory file listing target nodes
├── playbook.yaml # Main playbook to copy and run the script
└── README.md # Project documentation (this file)

## 📌 Objective

The goal is to practice:

- Setting up a working Ansible project
- Using the `copy` module to copy a shell script to remote machines
- Setting executable permissions via the `mode` attribute
- Using the `shell` module to remotely execute the copied script

## ⚙️ Setup Steps
1. **Prepare the required files**:
   - `ansible.cfg` – to specify the inventory file.
   - `hosts.ini` – to define the target hosts and SSH user.
   - `hello.sh` – shell script that prints `Hello world`.
   - `playbook.yaml` – playbook to automate the copying and execution process.
2. **Run the playbook**:
   ```bash
   ansible-playbook playbook.yaml
