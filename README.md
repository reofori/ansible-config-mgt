# Ansible-Configuration-Management-Automate-Project-7-to-10-

## Step 1 - Install and Configure Ansible on EC2 Instance.

1. Update the Name tag on your Jenkins EC2 Instance to Jenkins-Ansible. We will use this server to run playbooks.

![image](images/0.png)

2. In  GitHub account create a new repository and name it ansible-config-mgt.

![image](images/1.png)

3. Install Ansible.

```
sudo apt install ansible -y
```
![image](images/2.png)

Check your Ansible version by running ansible --version

![image](images/3.png)

4. Configure Jenkins build job to archive repository content every time you change it - this will solidify Jenkins configuration skills acquired in Project 9.

Create a new Freestyle project 'ansible' in Jenkins and point it to 'ansible-config-mgt' repository.

![image](images/4.png)

Configure a webhook in GitHub and set the webhook to trigger ansible build.

![image](images/5.png)


Configure a Post-build job to save all (**) files, like you did it in Project 9.
![image](images/6.png)

