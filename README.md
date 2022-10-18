# PrestaShop Docker by Bitnami

## Start and install container
To start the container run  
`docker-compose up -d`  
using the terminal/powershell in the folder containing docker-compose.yml.  
  
View progress in Docker desktop -> go to container -> logs (Might take over 10 minutes to run first time).  
The container might quit when installations is done, just start it again if it happens.

## Folder name
Do not rename "prestashop-persistence" in docker-compose.yml, this folder name tells the installer that you want to mount the files.  
The path to /prestashop-persistence can be changed without problem

## Navigate to server
After installation is done, navigate to: http://localhost/

Admin:  
http://localhost/administration  
username: user@example.com  
password: bitnami1  

## Timeout issue
Add this line to increase the timeout to 100 seconds  
`ini_set('max_execution_time', 100);`  

In the end of C:\Users\DPJ\Desktop\bitnami-docker-prestashop\prestashop-persistence\config\config.inc.php

## More information
See https://github.com/bitnami/bitnami-docker-prestashop
