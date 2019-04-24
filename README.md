# ansible-ec2-nginx-docker

The code has been tested on Ubuntu 18.04.

The new instance also created with t2 micro Ubuntu 18.04.

The code will have a previous check before the instance and volume creation. 

On AWS side it will create security group, subnet, instance and volume.

Then install docker and run Nginx container

Use the curl get the html file of Nginx default page and store and file. Do strip after that. 

The last is use while loop to do the heanth check run every 10s and store in logs file.
