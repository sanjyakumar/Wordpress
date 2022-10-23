# install ansible/setup
for a fresh linux ec2 instance first install ansible master 
for install ansible master
check python version # python --version
update the server # yum update
install ansible package # amazon-linux-extras
check ansible # ansible --version
for ansible create a user # useradd ansadmin
set the password # passwd ansadmin
for sudo previlage add ansadmin to suofile 
uneble ssh password auth. # vim /etc/ssh/sshd_config
after chage config. restart the sshd service # service sshd restart
not required for install ansible in clint machine bcoz it is a ageintless tool / in clint must have python .
same as create a user ansadmin in clint machene and set password / add to visudo file .
in ansible master their was a inventory file called 'hosts'</etc/ansible>
under hosts file we define the ip of clint machine for the connection
it connected to clint over ssh so we need to establishd ssh connection

# for deploy a wordpress site we need prerequesites

HTTP.PHP,MYSQL must be instaled in the server
for install HTTP and PHP service first run lamp.yml file it is install php and http service 
then start the service HTTP and PHP
after that creat a mysql data 
for create the mysql database run mysql.yml file
then configure the data base
>mysql_sequre_instaletion
> set the root password: yes
     enter the password:
     re-enter the password:
Download database site
configure the wordpress with data base
open the config file 'wp-config-sample.php'
under that file we set the data base name
after that set username and database passwd 
check the DNS site
 
# Deploying a high-availability WordPress website using ELB
lunch a DB instance in amazon RDS
lunch a Launch an Elastic Beanstalk environment
store the wordpress file in s3 bucket then uplode and deploye the file

# Deploying a high-availability WordPress website Autosceling
set load balancing on the VPC for that use ALB
ALB besically work on the HTTP/HTTPS protocal
Create a AMI of the ansible master 
set Launch Configurations for that AMI 
set the autoscling group 

# for Dockerfile 
on ansible master run the Dockerfile it will be clone the repo inside the repo dir after that configure the data base first then run the wordpress.yml file.





