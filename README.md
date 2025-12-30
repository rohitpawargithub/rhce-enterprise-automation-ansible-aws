# RHCE Major Project – Enterprise Linux Automation using Ansible on AWS

## 📌 Overview
This project demonstrates RHCE-level skills by automating enterprise Linux server management on AWS EC2 using Ansible. It includes user management, Apache deployment, LVM automation, SELinux and firewall configuration, and scheduled backups using reusable Ansible roles.

---

## 🛠️ Technologies
- RHEL 8 / RHEL 9
- Ansible (Playbooks, Roles, Inventory)
- AWS EC2
- Apache (httpd)
- SELinux, firewalld
- LVM, XFS
- Git & GitHub

---

## 🏗️ Architecture
Ansible Control Node manages multiple EC2 instances using SSH.

---

## 📂 Roles Implemented
- users – User and group management
- webserver – Apache deployment
- lvm – Automated storage provisioning
- firewall – firewalld & SELinux configuration

---

## ▶️ How to Run
```bash
ansible-playbook playbooks/site.yml

## Project Structure

rhce-enterprise-automation-ansible-aws/
│
├── README.md
├── ansible.cfg
│
├── inventory/
│   └── aws_hosts.ini
│
├── playbooks/
│   ├── site.yml
│   ├── users.yml
│   ├── webserver.yml
│   ├── lvm.yml
│   ├── firewall_selinux.yml
│   └── backup.yml
│
├── roles/
│   ├── users/
│   │   └── tasks/main.yml
│   │
│   ├── webserver/
│   │   ├── tasks/main.yml
│   │   ├── handlers/main.yml
│   │   └── templates/index.html.j2
│   │
│   ├── lvm/
│   │   └── tasks/main.yml
│   │
│   ├── firewall/
│   │   └── tasks/main.yml
│
├── aws/
│   └── ec2-setup.md
│
└── screenshots/
    └── (add execution proof)

