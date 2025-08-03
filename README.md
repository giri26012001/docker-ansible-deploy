# docker-ansible-deploy

Task 1: Install required packages:
- Installs dependencies needed to enable https repositories, manage certificates, use curl to fetch docker GPG key.

Task 2: Add docker GPG key:
- Adds Docker’s GPG key to your system so that the system can verify Docker packages.

Task 3: Add Docker repository:
- Adds Docker's official apt repository to your system. focal refers to Ubuntu 20.04 (you can replace it with {{ ansible_distribution_release }} for dynamic detection).

Task 4: Install Docker:
- Installs the Community Edition of Docker (docker-ce) and ensures you have lates version.

Task 5: Ensure Docker is running:
- Starts Docker service if it’s not already running and ensures dokcer is started if server is rebooted.

Task 6: Pull Docker image:
- Pulls the latest image from Docker Hub.

Task 7: Run Docker container
- Starts a Docker container and maps port 70 to host port 70.
