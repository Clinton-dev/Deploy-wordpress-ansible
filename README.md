# WordPress Deployment with Nginx & Ansible

This project automates the installation and setup of WordPress with Nginx using Ansible. It configures security keys, sets up the database, and optimizes Nginx for WordPress.

## 🚀 Features

- **Automated WordPress installation**
- **Nginx configuration for optimal performance**
- **Secure `wp-config.php` setup**
- **Customizable variables** for domain, database, and security keys

## 🛠 Prerequisites

Before running the playbook, ensure you have:

- **Ansible installed** – Follow the [Ansible installation guide](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#id11) and use `pipx` for installation: `pipx install --include-deps ansible`. For more information on `pipx`, visit the [pipx documentation](https://pipx.pypa.io/stable/).
- **A Linux server** (Ubuntu/Debian recommended)
- **SSH access** to the server
- **A domain name** pointed to the server

## ⚙️ Setup & Usage

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-repo/wordpress-nginx-setup.git
cd wordpress-nginx-setup
```

### 2️⃣ Configure Variables
Edit `/vars/vars.yml` to set:

- **`domain_name`** – Your domain name
- **`db_name`**, **`db_user`**, **`db_password`** – Database credentials
- **Security keys** – Set manually or let the playbook generate them  

### 3️⃣ Run the Playbook
```sh
ansible-playbook wordpress_new_server_setup.yaml -i inventory.ini
```

### 4️⃣ Access Your Site
Visit [http://your-domain.com](http://your-domain.com) to complete the setup.  

## 📸 Screenshots

### WordPress Deployment in Action
![WordPress Setup](screenshots/wordpress-setup.png)


