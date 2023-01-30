# 1. Pendahupluan SQL

MySQL adalah Relational Database Management System (RDBMS) digunakan untuk mengolah data terstruktur. MySQL merupakan salah satu database yang paling banyak digunakan saat ini.

Database merupakan elemen penting dalam aplikasi karena mampu menyimpan data. Data yang tersimpan dapat digunakan kembali untuk berbagai kepentingan seperti ditampilkan, diagregasi, diolah dan sebagainya.

MySQL mampu menyimpan banyak database. Setiap database tersusun oleh table dan setiap table terdiri dari kolom (field) dan baris data (row).

![database](/img/tabledatabase-1024x615.png)
Hubungan antara Database, Table, Field dan Record


MySQL sudah terdapat dalam paket XAMPP dan siap digunakan setelah instalasi XAMPP sudah dilakukan.

### Cara menjalankan service MySQL

*Note : Pastikan anda sudah menginstall XAMPP*

Di **Windows**, Buka XAMPP control panel dan tekan tombol Apache dan MySQL
![xampp](/img/image-26.png)


Di **Linux**, ketik sudo /opt/lampp/lampp start

``` bash
$ sudo /opt/lampp/lampp start
 Starting XAMPP for Linux 7.1.26-1…
 XAMPP: Starting Apache…ok.
 XAMPP: Starting MySQL…ok.
 XAMPP: Starting ProFTPD…ok.
```
**MySQL** menggunakan bahasa SQL (Structured Query Language) untuk melakukan operasi data seperti menambah, merubah, menghapus dan sebagainya.

mengakses MYSQL bisa menggunakan GUI yaitu dengan `http://localhost/phpmyadmin/` dan bisa mengakses melalui terminal / command prompt.

#### di linux

```
cd /opt/lampp/bin/
./mysql -u root -p
```

#### di windows

```
cd c:\xampp\mysql\bin 
mysql.exe -u root -p
```

Dalam SQL terdapat 5 istilah perintah untuk manipulasi data yaitu:

1. **Data Definition Language** (DDL)
2. **Data Manipulation Language** (DML)
3. **Data Query Language** (DQL)
4. **Data Control Language** (DCL)
5. **Transaction Control Language** (TCL)

### DDL, DML, DQL, DCL, TCL

**Data Manipulation Language** (DML) adalah perintah SQL untuk manipulasi data dalam table

**Data Query Language** (DQL) adalah perintah SQL untuk query data

**Data Control Language** (DCL) adalah perintah SQL untuk kontrol dan permission database

**Transaction Control Language** (TCL) adalah perintah SQL yang berhubungan dengan transaksi di database
