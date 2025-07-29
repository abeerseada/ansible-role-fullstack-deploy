# fullstack_deploy (Ansible Role)

![Ansible](https://img.shields.io/badge/Ansible-Role-blue?style=flat-square)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

## Description

This Ansible role deploys a complete **fullstack web application** using:

- **Node.js** (backend)
- **Nginx** (reverse proxy)
- **Systemd service** for process management

It sets up the environment, installs dependencies, and ensures the app is served via Nginx on port 80.

---

## Requirements

- Ubuntu 20.04 or 22.04
- Ansible 2.9+
- Node.js & npm installed via the role
- SSH access to the target host

---

## Role Variables

You can customize the following variables (see `defaults/main.yml`):

```yaml
app_user: "nobody"
app_group: "nogroup"
app_port: 3000
app_dir: /var/www/todo-app


Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
# ansible-role-fullstack-deploy
