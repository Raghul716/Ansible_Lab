# Ansible_Lab

# In main branch 

# A1 
Tasks To Be Performed: 
1. Setup Ansible cluster with 3 nodes 
2. On slave 1 install Java 
3. On slave 2 install MySQL server 
Do the above tasks using Ansible Playbooks

# A2
Tasks To Be Performed:
1. Create a script which can add text “This text has been added by custom
script” to /tmp.1.txt
2. Run this script using Ansible on all the hosts

# A3
Tasks To Be Performed:
1. Create 2 Ansible roles
2. Install Apache2 on slave1 using one role and NGINX on slave2 using the
other role
3. Above should be implemented using different Ansible roles

# A4
Tasks To Be Performed:
1. Use the previous deployment of Ansible cluster
2. Configure the files folder in the role with index.html which should be
replaced with the original index.html
All of the above should only happen on the slave which has NGINX installed
using the role

# A5
Tasks To Be Performed:
1. Create a new deployment of Ansible cluster of 5 nodes
2. Label 2 nodes as test and other 2 as prod
3. Install Java on test nodes
4. Install MySQL server on prod nodes
Use Ansible roles for the above and group the hosts under test and prod

# Case Study
Problem Statement:
You are a DevOps Engineer and the organization you are working on needs to
set up two configuration management server groups. One for Apache, another
for NGINX. Being a DevOps Engineer it is your task to deal with this
configuration management issue.
Let us see the tasks that you need to perform using Ansible:
1. Create two server groups. One for Apache and another for NGINX
2. Push two html files with their server information
Make sure that you don’t forget to start the services once the installation is done.
Also send post installation messages for both the server groups.
Using Ansible roles accomplish the above tasks. Also, once the Apache server
configuration is done you need to install Java on that server group using Ansible
role in a Playbook.
