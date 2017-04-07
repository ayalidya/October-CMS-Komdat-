# October-CMS-Komdat-
Projek ini untuk tugas akhir mata kuliah Komunikasi Data dan Jaringan  
***

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
***

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
### 6. Buat database baru untuk October CMS di mysql dan ubah status kepemilikannya
```shell
create database nama_database character set utf8;
GRANT ALL PRIVILEGES ON nama_database.* TO 'nama_database'@'alamat_server' IDENTIFIED BY 'password_database'
flush privileges;
```

### 7. Atur database, administrator, dan backend environment
Masuk ke browser dan ketikkan alamat http://172.18.88.85/install.php
Atur database dan arahkan ke database yang telha dibuat sebelumnya.

![GitHub Logo](/images/Capture1.PNG)

Klik tombol administrator. Masukkan identitas untuk admin: nama, password, dan yang lainnya

![GitHub Logo](/images/Capture2.PNG)

Klik tombol advanced. Masukkan URL untuk mengakses sistem admin.

![GitHub Logo](/images/Capture3.PNG)

***
# Post-Installation
Hapus file 'install.php' dan folder 'install-master' dari directory

![GitHub Logo](/images/Capture4.PNG)
