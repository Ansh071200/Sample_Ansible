# 🌟 Installing Ansible and Deploying a Playbook to a Web Server on EC2

## Make sure you have the EC2 Instance configured.

## 🐧 Procedure to Install Ansible on Ubuntu


1. **Update the apt package index:**

``` bash
sudo apt update
sudo apt upgrade
```

2. **Install Ansible:**

``` bash
sudo apt install ansible
```

3. **Check Ansible version:**

``` bash
ansible --version
```

4. **Clone this Repository:**

``` bash
git clone https://github.com/Ansh071200/Sample_Ansible.git
cd Sample_Ansible
```

5. **Run the Playbook:**

``` bash
ansible-playbook ansible_playbook.yml
```

6. **Expose the URL:**

   **-> Check the port number and the Service status**

``` bash
sudo systemctl status apache2
sudo cat /etc/apache2/ports.conf | grep Listen
```
   **->Change the inbound rules of the instance security group to the designated port on which the server is running.**
![Change the Inbound rules](https://github.com/Ansh071200/Sample_Ansible/blob/main/image_2024-07-17_192901543.png)
   

7. **Open the browser and type your public EC2 DNS followed by the Port number.:**

-> http://your-ec2-public-dns:8080


