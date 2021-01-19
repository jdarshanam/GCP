# GCPTrain - Startup Script for Load Balancer Test - HTTP. 

For USA 

#! /bin/bash

sudo apt-get update

sudo apt-get install wget
sudo apt-get install python

wget https://raw.githubusercontent.com/jdarshanam/GCP/main/LoadBalancerDemo/frontend-uswest.py

sudo python frontend-uswest.py &


.


For  Asia 

#! /bin/bash

sudo apt-get update

sudo apt-get install wget
sudo apt-get install python

wget https://raw.githubusercontent.com/jdarshanam/GCP/main/LoadBalancerDemo/frontend-asia.py

sudo python frontend-asia.py &


.


For  Europe 

#! /bin/bash

sudo apt-get update

sudo apt-get install wget
sudo apt-get install python

wget https://raw.githubusercontent.com/jdarshanam/GCP/main/LoadBalancerDemo/frontend_europe.py

sudo python frontend_europe.py &


############################################################################


Curl Command

Slow 

while true ; do (curl http://[Load Balancer ExternalIP]/service ) ; sleep 2 ; done 


Fast

while true ; do (curl http://[Load Balancer ExternalIP]/service ) ; sleep 0.1 ; done 


