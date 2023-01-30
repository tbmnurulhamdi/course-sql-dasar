# 6. DQL Filtering WHERE

Jika kita ingin menampilkan hanya data yang memenuhi kriteria tertentu saja, maka dapat dilakukan dengan menambah perintah WHERE pada query SELE
Format dasar query SELECT…WHERE adalah:
```
SELECT field1, field2, field3, ...
FROM nama_table
WHERE kondisi
```
Misal mencari data mahasiswa yang bernama anto
```
SELECT * FROM mahasiswa WHERE nama="anto";
```
Kondisi WHERE sangat fleksibel dan kita bisa menggunakan berbagai operasi kondisi seperti lebih besar (>), lebih kecil (<), tidak sama (<>), dan lain-lain.

operasi logika
| Operator   | Penjelasan    |
|--------------- | --------------- |
| NOT atau !   |  Logika bukan  |
| AND atau &&   |  Logika dan   |
| OR atau |  Logika atau   |
| XOR   |  Logika bukan atau (XOR)   |

Operasi Perbandingan
| Operator   | Penjelasan    |
|--------------- | --------------- |
| =   |  Sama dengan  |
| <> atau !=   |  Tidak sama dengan  |
| <=>   |  sama dengan (null safe)  |
| <   |  kurang dari  |
| <=   |  kurang dari atau sama dengan  |
| >   |  lebih besar dari  |
| >=   |  lebih besar atau sama dengan  |
| BETWEEN   |  Berada pada batas tertentu  |
| IN   |  Berada di dalam  |
| IS NULL   |  Pengecekan apakah berisi NULL  |
| IS NOT NULL   |  Pengecekan apakah bukan berisi NULL  |
| LIKE   |  Pencarian menggunakan wildcard  |
| REGEXP atau RLIKE   |  Pencarian menggunakan Regular Expression  |

Contoh, mencari data mahasiswa yang bernama anto dan beralamat semarang
```
SELECT * FROM mahasiswa WHERE nama="anto" AND alamat="semarang";
```
Operator **AND** akan menghasilkan nilai TRUE jika kedua pernyataan bernilai benar dan FALSE jika salah

Jika kita mencari data mahasiswa yang bernama anto atau mahasiswa yang beralamat jakarta
```
SELECT * FROM mahasiswa WHERE nama="anto" OR alamat="jakarta";
```
Maka dengan operator **OR** akan dicari data mahasiswa yang bernama anto dan mahasiswa yang berasal dari jakarta

Operator **NOT** akan menghasilkan nilai TRUE jika pernyataan bernilai salah. Contoh, mencari data mahasiswa yang tidak bernama anto
```
SELECT * FROM mahasiswa WHERE NOT nama="anto";
```

Klausa WHERE dapat dikombinasikan dengan operator **LIKE** untuk mencari data yang lebih spesifik berdasarkan pola. Contoh, Mencari data mahasiswa yang mempunyai nama dengan pola ‘an’
```
SELECT * FROM mahasiswa WHERE nama LIKE '%an%';
```


