# October-CMS-Komdat-
Projek ini untuk tugas akhir mata kuliah Komunikasi Data dan Jaringan


Step:

0.  install 
    sudo apt install apache2
    sudo apt install mysql-server
    sudo apt install php7.0
    sudo apt install libapache2-mod-php
    sudo apt install php7.0-mysql
    sudo apt install php7.0-gd php7.0-mcrypt php7.0-mbstring php7.0-xml php7.0-ssh2
    sudo service apache2 restart
    
2. Install PDO PHP Extension -> sudo apt-get install php7.0-mysql 
3. Install cURL PHP Extension -> sudo apt-get install php7.0-curl
4. Install OpenSSL PHP Extension 
5. Install Mbstring PHP Library -> sudo apt-get install php7.0-mbstring
6. Install ZipArchive PHP Library -> sudo apt-get install php7.0-zip
7. Install GD PHP Library 
8. Download binary file dari website octobercms.com/download -> sudo wget http://octobercms.com/download
9. Pindahkan kan file download.zip dari folder download ke folder parentnya -> sudo mv download download.zip
10. Unzip file download.zip -> sudo unzip download.zip
11. Copy file semua file yang berada di folder install-master dan paste ke direktori

![GitHub Logo](/images/Capture1.PNG)

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

### 2. Instal package yang dibutuhkan untuk menginstall **October CMS**
##### PDO PHP Extension
```shell
sudo apt-get install php7.0-mysql
```

##### cURL PHP Extension
```shell
sudo apt-get install php7.0-curl
```

##### Mbstring PHP Library
```shell
sudo apt-get install php7.0-mbstring
```

##### ZipArchive PHP Library
```shell
sudo apt-get install php7.0-zip
```

##### GD PHP Library 
```shell
sudo apt-get install php7.0-gd
```

# Installing October CMS
### 1. Download installation file pada halaman http://octobercms.com/download
```shell
sudo wget http://octobercms.com/download
```

### 2. Pindahkan file download ke download.zip
```shell
sudo mv download download.zip
```

### 3. Ekstrak file download.zip
```shell
sudo unzip download.zip
```

### 4. Copy semua file yang berada pada folder "install-master" dan masukkan ke "/var/www/html/"
```shell
sudo cp -r ~/install-master/* /var/www/html/
```

### 5. Setting permission dan ganti kepemilikan dari folder "/var/www/html/"
```shell
sudo chown -R www-data:www-data /var/www/html/
sudo chmod -R 755 /var/www/html/
```
