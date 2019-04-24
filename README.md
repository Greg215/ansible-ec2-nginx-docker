# ansible-ec2-nginx-docker


The new instance also created with t2 micro Ubuntu 18.04.

The code will have a previous check before the instance and volume creation. 

On AWS side it will create security group, subnet, instance and volume.

Then install docker and run Nginx container

Use the curl get the html file of Nginx default page and store and file. Do strip after that. 

The last is use while loop to do the heanth check run every 10s and store in logs file.

# Requriement to run this code:

Ubuntu 16 and above, this code has been etsted on 18.04. 
Add ansible_python_interpreter=/usr/bin/python3 as Ansibe default uses python2, and new Ubuntu default has python3.
Install Boto and boto3 for python3, add the aws key and secret to aws configure. 
Create an Ansible vault .vault-pass.txt with the private key, key variable name: private_key. 
Change the AWS relate variable like region, CIDR of subnet, image id etc if not in eu-west-1 region.


