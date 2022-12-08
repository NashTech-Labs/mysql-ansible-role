### What will this role do ?

The above package role will help you install mysql on any server. This role will install and configure mysql on any machine. It will also help you in as :

1. In the install.yml file , first it will add mysql apt key and after add it will install all the mysql packages and checks that mysql is installed.

2. Further in the configure.yml file it will update and configure the my.conf to /etc/mysql/my.cnf . 




#### Variable used in the role 


* mysql_port: Here in this variable you need to put your mysql port.

* mysql_bind_address: In this give you mysql bind address.

* mysql_language: It refers to the path of the mysql package.

* mysql_ppa:  Put your know ppa key.

* mysql_apt_key: Give your own mysql apt key.

* mysql_packages: THis will include all the packages that you will need to install mysql.




### How to run the playbook 

To run the playbook follow the below command:-

`ansible-playbook -i <your inventory file> playbook.yml`

**Note**:-  If you are running on your local system then you don't need to pass inventory file. Just use localhost in hosts of playbook. 