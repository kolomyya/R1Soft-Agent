# R1Soft-Agent

This file will help you to install R1Soft Agent into CentOS6, CentOS7, Fedora, Debian and Ubuntu.
Line 33 and 90 needs to be changed to your R1Soft Server's IP Address.


Installing R1soft agent on CentOS6, CentOS7 and Ubuntu
This ansible playbook will install R1soft agent. Please follow the steps

Step 1 Create r1soft server

Step 2 Copy ssh key from the R1soft server to the remote hosts ssh-copy-id

Step 3 Add hosts to the inventory file

cat hosts
[r1soft]
youripaddress

Step 4 Run the playbook

git clone https://github.com/kolomyya/R1Soft-Agent.git
cd r1soft-ansible
ansible-playbook -i hosts r1soft.yml
