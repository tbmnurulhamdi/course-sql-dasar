# 8. DML DELETE

Untuk penghapusan baris (atau disebut juga dengan record) dalam MySQL, kita memerlukan beberapa syarat, yaitu nama tabel dimana baris tersebut berada serta kondisi untuk penghapusan.
```
DELETE 
FROM nama_table 
WHERE kondisi
```
Contoh kita akan menghapus record dengan NIM = 21400200
```
DELETE 
FROM mahasiswa 
WHERE nim="21400200"
```
Kunci dari query DELETE ada di pernyataan kondisi setelah WHERE, yaitu dimana kita memberitahukan MySQL syarat/kondisi yang harus dipenuhi untuk menghapus suatu record. Biasanya berdasarkan primary key.
