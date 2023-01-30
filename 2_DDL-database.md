# 2. Perintah DDL pada Database

**Data Definition Language (DDL)** merupakan perintah SQL untuk membuat, merubah atau menghapus struktur database.

Perintah DDL pada databse antara lain:
```
SHOW -> Melihat database
CREATE -> Membuat database
USE -> memilih database
DROP -> Menghapus database
```
### perintah SHOW

perintah ini digunakan untuk melihat database-database yang ada pada MYSQL

**Melihat database**
```
show databases;
```

### perintah CREATE

**Membuat Database**
```
CREATE DATABASE nama_database;
```

Contoh membuat database **universitas**
```
CREATE DATABASE universitas;
```

### perintah USE

Sebelum membuat table, kita harus memilih database yang akan di eksekusi yaitu dengan perintah **use**

**memilih database**
```
use nama_database;
```
Contoh memilih database **universitas**
```
use universitas;
```

### perintah DROP

saat kita tidak menginginkan database yang telah dibuat kita bisa menghapusnya. perlu diperhatikan saat penghapus database jangan sampai kita menghapus database penting.

**menhapus database**
```
DROP DATABASE nama_database;
```
