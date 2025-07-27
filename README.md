# docker-ansible-deploy
Deploying a Dockerized application using Ansible

Below are the steps explained for main.yml tasks:
Task 1: update apt cache:
- updates the apt package. It's equivalent to "sudo apt update".
  
Task 2: Install packages:
- Installs dependencies to enable HTTPS, manage certificates, curl to fetch docker GPG keys and to manage and add apt-repositories.

Task 3: Add docker GPG key:
- Adds Docker’s GPG key to your system so that the system can verify Docker packages and prevents installing tampered packages.

Task 4: Add Docker repo:
- Adds Docker's official apt repository to your system. 
