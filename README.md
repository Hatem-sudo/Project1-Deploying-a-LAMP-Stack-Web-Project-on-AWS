# Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS
## WEB STACK IMPLEMENTATION (LAMP STACK) IN AWS 
### AWS account setup and provisioning an Ubuntu Server
#### Steps


1. Launched an EC2 instance
2. I selelected the Ubuntu free tier instance
3. I set the required configurations (Enabled public IP, security group, and key pair) and finally launched the instance.
![project1pix3](https://user-images.githubusercontent.com/74002629/174606543-32845537-efdd-4abe-a903-82a20f3bbb80.PNG)

4. Next I SSH into the instance using Windows Terminal

![project1pix5](https://user-images.githubusercontent.com/74002629/174608722-755ce47c-4c8e-475c-a399-43e314235364.PNG)

### INSTALLING APACHE AND UPDATING THE FIREWALL

#### Steps


1. Install Apache using Ubuntu’s package manager :
2. To run apache2 package installation:
3. Next, verify that Apache2 is running as a service in the OS. run:
4. The green light indicates Apache2 is running.
   
![1](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/360f6b38-63da-4d02-aea4-ae4589aa61c5)

6. Open port 80 on the Ubuntu instance to allow access from the internet.
7. Access the Apache2 service locally in our Ubuntu shell.
8. Next, test that Apache HTTP server can respond to requests from the Internet. Open a browser and type the public IP of the Ubutun instance: **http://3.235.248.184/:80** This outputs the Apache2 default page.
   
![2](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/5fc5af2c-4b59-472a-8b47-916b151a2e44)

![3](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/0bcad80d-1c3c-4352-9346-1dfe5ae712d3)



### INSTALLING MYSQL

#### Steps



In this step, I install a Database Management System (DBMS) to be able to store and manage data for the site in a relational database.
1. Confirm intallation.
2. Once installation is complete, log in to the MySQL console.
3. Next, run a security script that comes pre-installed with MySQL, to remove some insecure default settings and lock down access to your database system.
4. Run interactive script by typing.
5. Next, test that login to MySQL console works
![6 install mysql](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/74253c5b-b54f-4069-ad69-b750363aac4e)
6. Type exit and enter to exit console.

### STEP 3 — INSTALLING PHP

#### Steps


1. install these 3 packages php libapache2-mod-php php-mysql.
2. LAMP stack is completely installed and fully operational.
![7 mysql](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/1caf3827-133d-4205-ad48-60ea91367c03)

### STEP 4 — CREATING A VIRTUAL HOST FOR YOUR WEBSITE USING APACHE

#### Steps



1. Setting up a domain called projectlamp.
2. assign ownership of the directory with your current system user.
3. a new configuration file in Apache’s sites-available directory.
4. Edite Configration file .

  ![8 9 10](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/173a87b7-05cb-495f-b79f-93855fea4899)
  
5. Enable the new virtual host.
6. Disable the default website that comes installed with Apache.
7. Finally, reload Apache so these changes take effect: **sudo systemctl reload apache2**
  ![11 12 13](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/3504193b-47d8-44ba-b4d4-83e8373d14dc)

#### Congratulition The website is active ..

![14](https://github.com/Hatem-sudo/Project1-Deploying-a-LAMP-Stack-Web-Project-on-AWS/assets/113099054/a638e5c7-f992-4fbe-b7ea-f65963bfa12d)

