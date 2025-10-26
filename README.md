# Test Task — OpenVPN Web Deployment via Ansible

This project provides an **Ansible-based automation** for deploying **OpenVPN** on a remote or local host (for example, on **Azure**, **AWS**, or **localhost**) and exposing a **web interface** that displays available `.ovpn` configuration files.

---

## 📦 Features

- Installs and configures **OpenVPN** on the target host.
- Exposes **port 1995** for accessing a web page that lists available VPN configuration files.
- Automatically places generated `.ovpn` configs in a visible web directory.
- Supports **multiple environments**:
  - Localhost  
  - Remote servers (Azure, AWS, or Linux host with SSH access)

---

## ⚙️ Requirements

- Ansible 2.12+
- SSH access to target host
- Linux distribution supported by your Ansible roles (Ubuntu, Debian, CentOS, Fedora)

No external Python or system dependencies are required.

---

## 🚀 Usage

Run the main playbook:

```bash
ansible-playbook playbook.yaml --extra-vars "target=localhost"
