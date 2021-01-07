# Provisioning-and-Configuration-of-instances-over-AWS-using-Ansible
This Repository will help you to provision instances over AWS and configure them using Ansible. Here the use case is to configure reverse proxy on AWS cloud.
<h2> How to use this Playbook </h2>
<p> 1.To use this Playbook first clone the repository </p>
<p> 2.Create a file containing the Access key and Secret key using Ansible Vault </p>
<p> To do this use this command: </p>
<h4> ansible-vault create "name of your file" </h4>
<p> Use the variables access_key and secret_key for your Access key and Secret key respectively. </p>
<p> 3.Next run the setup.yml file using the command </p>
<h4> ansible-playbook setup.yml </h4>
<p> 4.Now export the system variables AWS_REGION, AWS_ACCESS_KEY and AWS_SECRET_ACCESS_KEY. </p>
<p> 5.Run the ec2.py file </p>
<p> 6.Set become=true, become_method , become_user and become_ask_pass=false </p>
<p> 7.Next you just need to run config_server.yml file using this command </p>
<h4> ansible-playbook config_server.yml </h4>
