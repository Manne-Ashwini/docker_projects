# Docker Projects
This repository contains various Docker projects and examples.

## Setup Docker on EC2 Instance

Follow these steps to set up Docker on an EC2 instance:

1. *Create EC2 Instance and Login*: Create an EC2 instance and log in to it using SSH.

2. *Update Packages*: Run the following command to update the package repositories:
   ```bash
   sudo apt update

Steps:

1 Install Docker: Install Docker using the following command:
sudo apt install docker.io -y

2 Check Docker Status: Verify the status of the Docker service using:
sudo systemctl status docker

3 Start Docker Service (if necessary): If Docker is not in the start state, use the command:
sudo systemctl start docker

4 Run hello-world Container: Test Docker installation by running a hello-world container:
docker run hello-world

5 Add User to Docker Group: Add the current user to the Docker group with the command:
sudo usermod -aG docker $USER

6 Logout and Login Again: Logout and login again for the group membership changes to take effect.

7 Run hello-world Container Again: After logging back in, verify Docker setup by running:
docker run hello-world
