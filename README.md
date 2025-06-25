# Nix DevOps Final Project
The goal of this project is to deploy and manage the infrastructure for the browser-based game Serpent Surge using modern DevOps tools and practices.

### Project Overview
The project implements a fully automated infrastructure setup to deploy the Serpent Surge game. It uses a variety of tools and services to achieve the following:

Linux Service for MySQL Backup (Task 1):
A Linux service was created to automatically back up a specific MySQL database table every day, with manual and automated archiving of backups every 3 days. The service also provides a command to list backup archives.

MySQL Database Setup (Task 2):
A MySQL database (serpent_surge_db) was created with a scores table containing player data, including id, name, score, and difficulty. A MySQL user was also created with restricted privileges to the database.

Git Setup and Repository Management (Task 3):
The project was pushed to a private GitHub repository, with a well-structured directory layout to include components for Ansible, Docker, and Terraform. A descriptive README was also included for project documentation.

### Installation and Setup - Prerequisites

1. Docker
2. Docker Compose

### Running the Application Locally
Clone the repository:

git clone https://github.com/nijiinhell/nix-devops-final.git
cd nix-devops-final/docker/serpent-surge-main
sudo docker-compose up --build 


The frontend will be available at http://localhost:3000, and the backend API will be running on http://localhost:5000.
