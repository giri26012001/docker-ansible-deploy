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
- Adds Docker's official apt repository to your system. {{ ansible_distribution_release }} is for you ubuntu release version. There are two release version focal and Jammy. Focal is used for Ubuntu 20.04 and Jammy is used for Ubuntu 22.04.

Task 5: Install docker:
- Installs the Community Edition of Docker. PLease ensure you always get latest version.

Task 6: Docker service running:
- Once you have installed docker ensure docker service is running on you server and enable it to auto-start when the server is booted.

Task 7: Pull image:
- pulls the lates image from docker hub.

Task 8: Run container:
- Starts the container and maps the port 80 to host port 80.
