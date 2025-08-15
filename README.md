# E-Commerce Web App (Bash-Driven Deployment)

This repository contains **both** the source code of a training e-commerce web application and the **Bash deployment script** used in the KodeKloud Bash-Scripting course (DevSecOps track).

The project simulates a real-world scenario where a Security/DevOps engineer automates the provisioning of the full stack: firewall, database, web server, application code, and validation.  
It is intended for **advanced** learners who want to integrate Bash scripting with DevSecOps and SOC workflows.

---

## 🚀 What It Does

- Installs and configures required packages:
  - `firewalld`
  - `mariadb-server`
  - `httpd` (Apache)
  - `php` / `php-mysql`
  - `git`
- Initializes the application database (creates DB, user, and populates sample data)
- Deploys the web app code to `/var/www/html/`
- Updates configuration files using `sed`
- Verifies the deployment (`curl` + product keyword check)

---

## 🔧 Usage

```bash
chmod +x deploy_ECommerce_Application.sh
sudo ./deploy_ECommerce_Application.sh
