# 4. DQL SELECT

Data Query Language (DQL) adalah perintah SQL untuk query data.
Perintah DQL yaitu
```
SELECT -> digunakan untuk melakukan query data dari database
```
Cara penulisan perintah SELECT
```
SELECT field1, field2, field3, ...
FROM nama_table; 
```
Jika ingin membaca semua field table gunakan tanda bintang (*)
```
SELECT * 
FROM nama_table;
```
Jika hanya ingin menampilkan beberapa atribut dari mahasiswa maka harus ditentukan field yang ingin di- SELECT. Contoh:
```
SELECT nama, alamat FROM mahasiswa;
```