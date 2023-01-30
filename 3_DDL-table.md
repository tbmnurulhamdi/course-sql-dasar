# DDL pada Table

**Data Definition Language (DDL)** merupakan perintah SQL untuk membuat, merubah atau menghapus struktur table.

Perintah DDL pada table antara lain:
```
SHOW -> Melihat table
CREATE -> Membuat table
ALTER -> Merubah struktur table
TRUNCATE -> Menghapus semua record di table
DROP -> Menghapus table/table
RENAME -> Merubah nama table
```
### perintah SHOW

setelah kita memilih database yang akan kita eksekusi, untuk melihat isi database kita menggunakan
perintah ini
```
show tables;
```

### perinth CREATE

Database berisi table untuk menyimpan entitas. Table terdiri dari field (kolom) dan record (baris data). Perintah CREATE digunakan untuk membuat table
**PRIMARY KEY** digunakan sebagai identifier unik untuk setiap record dan tidak boleh mengandung nilai NULL
**AUTO_INCREMENT** digunakan untuk menetapkan nomor urut secara otomatis. 
```
CREATE TABLE nama_table
(
    field1 tipe_data NOT NULL AUTO_INCREMENT,
    field2 tipe_data,
    field3 tipe_data,
    PRIMARY KEY(field)
)
```
Karena PRIMARY KEY harus bernilai unik maka untuk table mahasiswa yang bisa digunakan sebagai PRIMARY KEY adalah field NIM. Tetapi dicontoh ini kita tidak akan menggunakan AUTO_INCREMENT
Contoh
```
CREATE TABLE mahasiswa
(
    nim INT(10) NOT NULL,
    nama VARCHAR(100) NOT NULL,
    alamat VARCHAR(100) NULL,
    PRIMARY KEY(nim)
)
```
Kita telah membuat table mahasiswa dengan 3 field
```
INT(10) -> tipe data integer dengan maksimal 10 digit angka
VARCHAR(100) -> tipe data varchar dengan maksimal 100 karakter
NULL -> field diperbolehkan kosong
NOT NULL -> field tidak diperbolehkan kosong
```
Tipe data digunakan untuk mendefinisikan tipe dari field di table. Beberapa tipe data yang sering digunakan.
| tipe data   | keterangan    |
|--------------- | --------------- |
| INT   | Menyimpan nilai integer/numerik   |
| FLOAT   | Menyimpan nilai float   |
| VARCHAR   | Menyimpan nil;ai string   |
| CHAR   | Menyimpan nilai satu karakter   |
| DATE   | Menyimpan nilai waktu   |
| TEXT   | Menyimpan nilai teks   |
| BOOLEAN   | Menyimpan nilai boolean (true/false)   |

Untuk lebih jelasnya mari kita melihat di dokumentasi MYSQL [tipe data](https://dev.mysql.com/doc/refman/5.7/en/data-types.html)

### perintah ALTER

Perintah ALTER Untuk merubah struktur table seperti menambah, merubah, menghapus kolom

**Menambah kolom table**
```
ALTER TABLE nama_table 
ADD nama_field tipe_data
```
Contoh menambah field nomor telpon di table mahasiswa
```
ALTER TABLE mahasiswa 
ADD no_telp INT(15)
```

**Modifikasi kolom table**
```
ALTER TABLE nama_table 
MODIFY COLUMN nama_field tipe_data
```
Contoh merubah tipe data alamat dari varchar(100) menjadi text
```
ALTER TABLE mahasiswa
MODIFY COLUMN alamat TEXT
```

**Menghapus kolom table**
```
ALTER TABLE nama_table 
DROP nama_field
```
Contoh menghapus field nomor telepon
```
ALTER TABLE mahasiswa 
DROP umur
```

### perintah TRUNCATE

Perintah TRUNCATE digunakan untuk menghapus semua record di database
```
TRUNCATE TABLE nama_table
```
Misal tabel mahasiswa telah mempunyai record dan kita ingin menghapus recordnya
```
TRUNCATE TABLE mahasiswa
```

### perintah DROP

Perintah DROP digunakan untuk menghapus table
```
DROP TABLE nama_table
```

### perintah RENAME

Perintah RENAME digunakan untuk merubah nama table
```
RENAME TABLE nama_table_lama to nama_table_baru
```
Contoh merubah table mahasiswa menjadi siswa
```
RENAME TABLE mahasiswa to siswa
```