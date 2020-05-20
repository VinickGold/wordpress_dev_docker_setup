#### Minimum required docker setup to run a wordpress development environment

- Clone this repository and execute:
    ``` docker-compose up -d ``` 

Wordpress should be runing on localhost:8081 or the port you have specified in the docker-compose.yml file after some minutes.

- To stop all containers use: 
    ``` docker-compose down ```



You may want add this lines in .htaccess in order to be able to install heavy themes or plugins through wp user interface 
```
php_value upload_max_filesize 64M
php_value post_max_size 64M
php_value max_execution_time 300
php_value max_input_time 300
``` 