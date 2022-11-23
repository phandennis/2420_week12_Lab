# ACIT 2420 Week 12 Lab 

## Team member(s)
ByeongJu(Jace) Kang  
Dennis Phan

## Setting up NGINX on a server
This is a guide on how to install NGINX on a server with a firewall

### Step 1

Install NGINX on the server by following these instructions:

1. Run the command `sudo apt upgrade`


    ![sudo apt upgrade command](./image/apt_upgrade.PNG)


2. Run the command `sudo apt install nginx`
 
 
    ![Install Nginx with the command sudo apt install nginx](./image/install_nginx.PNG)


3. Run the command `sudo systemctl status nginx`


    ![checking the status of nginx to verify it is working properly](./image/nginx_status.PNG)


### Step 2

Use the HTML document in the repository and place it into `/var/www/your_ip/html/`

### Step 3

Use the NGINX server block file to serve the HTML.

### Step 4

1. Move your files to your 
![Uploading files to the server and appropriate directories](./image/move_files.png)

2. Creating a soft link to new server block in sites-enabled `sudo ln -s /etc/nginx/sites-available/your_ip /etc/nginx/sites-enabled/`
   Where `your_ip` is the ip of your server
3. Verify it works with `sudo nginx -t`  
![Verifying nginx configuration is working](./image/create_symbolic_link.png)

### Step 5

![Picutue 1](images/picture1.png)

### Step 6

![Picutue 1](images/picture1.png)

### Step 7

![Picutue 1](images/picture1.png)

### Step 8

![Picutue 1](images/picture1.png)
