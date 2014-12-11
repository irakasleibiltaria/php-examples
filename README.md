#PHP

[w3schools](http://www.w3schools.com/php/)

[http://php.net/manual/](http://php.net/manual/)

###Servers

MAC 

[https://bitnami.com/stack/mamp](https://bitnami.com/stack/mamp)

Windows 

[http://www.wampserver.com/](http://www.wampserver.com/)

[https://www.apachefriends.org](https://www.apachefriends.org)

Portable: [http://www.usbwebserver.net/en/](http://www.usbwebserver.net/en/) 

# Ubuntu server setup
```
sudo apt-get update
# apache + php + mysql
$ sudo apt-get install php5 mysql-server mysql-client php5-mysql

# port scanner
sudo apt-get install nmap
# nmap localhost
  
# git
sudo apt-get install git

# Sublime Text

## download http://www.sublimetext.com/2
#tar -xjvf Sublime\ Text\ 2.0.2.tar.bz2 
#cd Sublime\ Text\ 2/
##./sublime_text &

# OR
# http://www.ubuntuupdates.org/ppa/sublime_text_2
# http://www.ubuntuupdates.org/ppa/sublime_text_3

#sudo add-apt-repository ppa:webupd8team/sublime-text-3 
#sudo apt-get update
#sudo apt-get install <package name>

# chromium
sudo apt-get install chromium-browser
  
# config apache
cd /var/www/

sudo ln -s /home/zubiri/Documents/workspace/ workspace

# http://localhost/workspace

# PHP IDE: Aptana(eclipse + php) 
# java: http://openjdk.java.net/install/
$ sudo apt-get install openjdk-7-jre

# Download aptana http://www.aptana.com/  unzip and run

# Aptana php debug: Xdebug: http://digitaldisseny.com/en/blog/206-debug-php-aptana-ubuntu (TODO)
$ sudo apt-get install php5-xdebug

/etc/php5/apache2/conf.d/xdebug.ini

zend_extension=/usr/lib/php5/20090626/xdebug.so
 
xdebug.profiler_output_dir=/var/log/xdebug
xdebug.profiler_enable_trigger=1
xdebug.profiler_enable=0
 
xdebug.remote_enable=true
xdebug.remote_host=127.0.0.1
xdebug.remote_port=9000
xdebug.remote_handler=dbgp
xdebug.remote_autostart=0


Restart apache:
$ sudo apache2ctl graceful

```
