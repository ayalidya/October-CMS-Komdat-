# October-CMS-Komdat-
Projek ini untuk tugas akhir mata kuliah Komunikasi Data dan Jaringan

# Pre-installation
### 1. Install apache, mysql, php, dan package lain yang dibutuhkan pada server
```shell
sudo apt install apache2
sudo apt install mysql-server
sudo apt install php7.0
sudo apt install libapache2-mod-php
sudo apt install php7.0-mysql
sudo apt install php7.0-gd php7.0-mcrypt php7.0-xml php7.0-ssh2
sudo service apache2 restart
```
<br />
### 2. Instal package yang dibutuhkan untuk menginstall **October CMS**
##### PDO PHP Extension
```shell
sudo apt-get install php7.0-mysql
```
<br />
##### cURL PHP Extension
```shell
sudo apt-get install php7.0-curl
```

##### Mbstring PHP Library
```shell
sudo apt-get install php7.0-mbstring
```
<br />
##### ZipArchive PHP Library
```shell
sudo apt-get install php7.0-zip
```
<br />
##### GD PHP Library 
```shell
sudo apt-get install php7.0-gd
```
<br />
<br />
<br />
# Installing October CMS
### 1. Download installation file pada halaman http://octobercms.com/download
```shell
sudo wget http://octobercms.com/download
```
<br />
### 2. Pindahkan file download ke download.zip
```shell
sudo mv download download.zip
```
<br />
### 3. Ekstrak file download.zip
```shell
sudo unzip download.zip
```
<br />
### 4. Copy semua file yang berada pada folder "install-master" dan masukkan ke "/var/www/html/"
```shell
sudo cp -r ~/install-master/* /var/www/html/
```
<br />
### 5. Setting permission dan ganti kepemilikan dari folder "/var/www/html/"
```shell
sudo chown -R www-data:www-data /var/www/html/
sudo chmod -R 755 /var/www/html/
```
<br />
