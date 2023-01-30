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


