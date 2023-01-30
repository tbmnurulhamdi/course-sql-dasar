# 7. DML UPDATE

Query UPDATE dipakai untuk melakukan perubahan data pada tabel MySQL, yakni proses update baris atau record. Format dasar query UPDATE adalah sebagai berikut:
```
UPDATE nama_table
SET field1 = nilai1, field2 = nilai2, ...
WHERE kondisi;
```
Contoh kita ingin merubah alamat dari salah satu mahasiswa yang mempunyai NIM = 21400200
```
UPDATE mahasiswa
SET alamat = "surabaya"
WHERE nim="21400200"
```
Arti kode di atas adalah kita melakukan update table mahasiswa. Field yang dirubah adalah alamat mahasiswa yang mempunyai nim “21400200” (pakai petik karena string) menjadi surabaya

*note: perlu diperhatikan untuk tidak lupa klausa WHERE. bisa berdasarkan id, nim atau nama tetapi biasanya berdasarkan primary key*

