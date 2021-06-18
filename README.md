# ELK
Debian VM with Docker+Elasticsearch+Kibana

This repository includes 3 files for VMware, using this files u can run virtual machine with debian os.
Virtual machine already set up and ready for use.

To use the virtual machine you need user data:
root-user-login: User
root-user-pass: 019

Virtual machine has docker with elasticsearch and kibana, which located at /docker-elk

Important note: Elasticsearch has unique plugin jmorphy2. 

You can see plugin at GitHub : [jmorphy2](https://github.com/anti-social/jmorphy2)

# Run docker

To run docker u need to do 2 steps:

## Step 1. Getting ip.
First of all, for further work with elastic and kibana u will need ip adress, processing wia which u will get access.

Type in console : 
>ip a

Find in listed data field with 
><BROADCAST, MULTICAST, UP, LOWER_UP>

Usualy ip will start from: 
>192.168.0.0

## Step 2. Run Docker
First of all, to run docker, you need to go to the directory in which it is contained.
>cd /docker-elk

Now u can start docker using:
>sudo docker-compose up --build -d

## Connecting to Elasticsearch & Kibana
After setting up u can connect from your os to Elasticsearch & Kibana.

Just type in your browser ip adress from **Step 1.** and port  5601. 
Example:
>192.168.101.130:5601
