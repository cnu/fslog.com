---
title: Setting up LAMP on your Ubuntu desktop

date: 2006-12-01
url: /2006/12/01/setting-up-lamp-on-your-ubuntu-desktop/
categories:
  - Software

---
<img src="http://www.fslog.com/wp-content/uploads/2006/12/lamp.gif" id="image306" alt="lamp" align="right" />Many of you must be wanting to try some web development and would like to setup their own LAMP([Linux][1], [Apache][2], [MySQL][3], [PHP][4]/[Perl][5]/[Python][6]) stack. Ubuntu has a special [Server Edition][7] for setting up your own LAMP server, most of you may want to install it on your desktop (I like it that way).

This involves installing Apache, PHP, Python and MySQL. I think Python will be installed by default and we only need to install mod_python for Apache. I use Ubuntu Edgy Eft 6.10.

<!--more-->

**Apache 2**

Apache is the most popular web server and I use it for my development work. Apache 2 can be installed by running this command in the terminal.

`sudo apt-get install apache2`

All your files should be placed in the /var/www/ folder to be viewed from your server.

**PHP5**

PHP is on version 5 and can be installed by running

`sudo apt-get install php5<br />
sudo apt-get install libapache2-mod-php5<br />
sudo /etc/init.d/apache2 restart`

You can easily test whether you have correctly installed PHP by writing a simple test file.

`gksudo gedit /var/www/testphp.php`

This will open a text editor and here insert this line. There should be no space between < and ?. WordPress inserts a space in between.
  
`< ?php phpinfo(); ?>`
  
Point your browser to <http://localhost/testphp.php>

**MySQL Server**

Next install MySQL server

`sudo apt-get install mysql-server`

MySQL by default allows connections only from 127.0.0.1 i.e., only from your own computer. This is ok if you are developing only on your own system. If you want to access your MySQL server from a network,

`gksudo gedit /etc/mysql/my.cnf`

Find the line _bind-address = 127.0.0.1_ and comment it. Comments start with ;(semicolon).

If you want to set a different password to your MySQL server (than the default none),

`mysqladmin -u root password your-new-password<br />
mysqladmin -h root@local-machine-name -u root -p password your-new-password<br />
sudo /etc/init.d/mysql restart`

Install MySQL for Apache

`sudo apt-get install libapache2-mod-auth-mysql` `sudo apt-get install php5-mysql<br />
sudo apt-get install phpmyadmin`

After this, you have to enable the MySQL extension in your php.ini. Edit the file

`gksudo gedit /etc/php5/apache2/php.ini`

Here uncomment the line &#8220;_;extension=mysql.so_&#8221;

`extension=mysql.so`

After this restart Apache 2

`sudo /etc/init.d/apache2 restart`

**Python**

Python for Apache can be installed by installing the libapache2-mod-python package.

`sudo aptitude install python<br />
sudo aptitude install libapache2-mod-python`

 [1]: http://www.linux.org
 [2]: http://www.apache.org
 [3]: http://www.mysql.com
 [4]: http://www.php.net
 [5]: http://www.perl.com
 [6]: http://www.python.org
 [7]: http://www.ubuntu.com/server