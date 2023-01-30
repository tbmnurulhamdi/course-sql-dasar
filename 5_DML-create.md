# 5. DML CREATE(INSERT)

Data Manipulation Language (DML) adalah perintah SQL untuk manipulasi data dalam table. Kalau DDL fokus ke operasi struktur table/ database. sedangkan DML lebih fokus kepada operasi record data.

Perintah INSERT digunakan untuk menambah record data ke database.

Cara penulisan perintah INSERT
```
INSERT INTO nama_table (field1, field2, field3, ...)
VALUES (nilai1, nilai2, nilai3, ...);
```
Contoh kita lakukan penambahan data di table mahasiswa yang telah kita buat di materi DDL
```
INSERT INTO mahasiswa (nim, nama, alamat)
VALUES (21400200,"faqih","bandung")
```
Jika hanya beberapa field saja yang ingin dimasukkan maka nama field juga harus ditulis secara spesifik. Misal hanya field nim dan nama saja yang akan di-INSERT
```
INSERT INTO mahasiswa (nim, nama)
VALUES (21400200,"faqih")
```
Jika ingin memasukkan beberapa record sekaligus dapat ditulis dan setiap value dipisahkan dengen koma (,)
```
INSERT INTO mahasiswa 
VALUES 
(21400201,"ina","jakarta"),
(21400202,"anto","semarang"),
(21400203,"dani","padang");
```



