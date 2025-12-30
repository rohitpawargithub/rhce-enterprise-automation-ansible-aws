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
