# 9. DQL FILTERING ORDER BY & LIMIT

### ORDER BY
MySQL menyediakan perintah opsional ORDER BY untuk mengurutkan data yang di hasilkaN secara ascending (A-Z) atau descending (Z-A) Query dasar untuk SELECT…ORDER BY adalah
```
SELECT field1, field2, field3, ...
FROM nama_table
ORDER BY field1 | field2 | field3 ... ASC | DESC
```
Misal kita ingin menampilkan data mahasiswa berdasarkan nama terurut dari huruf A – Z
```
SELECT * FROM mahasiswa ORDER BY nama ASC;
```
Misal ingin menampilkan data mahasiswa yang mempunyai nama dengan pola ‘an‘ dan terurut dari huruf Z – A dengan kolom nama dan alamat saja
```
SELECT nama,alamat FROM mahasiswa WHERE nama LIKE '%an%' ORDER BY nama DESC;
```
Menggabungkan klausa WHERE dan operator LIKE dengan ORDER BY

### LIMIT
MySQL menyediakan pilihan opsional LIMIT untuk membatasi hasil query SELECT. Format dasar query SELECT…LIMIT adalah sebagai berikut:
```
SELECT field1, field2, field3, ...
FROM nama_table
LIMIT N
```
Misal kita ingin mencari data mahasiswa yang terurut berdasarkan nama sebanyak 3 teratas
```
SELECT * FROM mahasiswa ORDER BY nama ASC LIMIT 3;
```




