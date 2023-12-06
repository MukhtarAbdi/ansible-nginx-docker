# ansible-nginx-docker

How to Run the Ansible Playbook

Follow these steps to run the Ansible playbook on Ubuntu 22.04 EC2 instance with nginx docker container:

1.	Prerequisites:
•	Ensure that Ansible is installed on your local workstation. You can run the following command to install it:
# Update the system packages list:
sudo apt update -y

# Install the required dependencies:
sudo apt install software-properties-common -y

# Add the Ansible PPA (Personal Package Archive) to the system:
sudo apt-add-repository ppa:ansible/ansible

# Update the system packages list:
sudo apt update -y

# Install Ansible:
sudo apt install ansible -y

# To check the version of Ansible installed on your system, run the following command:
ansible –version
	
2.	Clone the Repository: To your local machine, clone the repository containing the Ansible playbook and README file:
git clone <repository-url>
cd <repository-directory>

3.	Inventory File: Create the inventory.ini file and save the IP address or hostname of your Ubuntu 22.04 EC2 instance.

4.	Ansible cfg File: Create the Ansible cfg file in your current directory.

5.	Run the Playbook: Run the Ansible playbook using the following command. It will prompt you for your Docker Hub username and password:
ansible-playbook -i inventory nginx_docker_playbook.yml

6.	Access Nginx: Once the playbook execution is complete, you can access the Nginx server by navigating to https://your_ec2_instance.

Note: Make sure to replace <repository-url> and <repository-directory> with the appropriate values. Additionally, replace your_ec2_instance with the actual IP address or hostname of your EC2 instance.

