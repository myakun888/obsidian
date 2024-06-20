# restore database
#mysql #restoredatabse #importdatabase
adalah perintah untuk mengembalikan database atau meginmport datase yang kita simpan untuk di masukan ke database kita saat ini

perintah nya 
ada dua cara 
### 1. cara dari queri mysqlnya
* buat database terlebih dahulu, sebagai tempat database nya
* masuk ke database yang akan kita restore / import datbase nya
* jalankan perintah ini `source lokasi_file_path_databasenya`, contoh file database nya disimpan pada folder datad, dengan nama db.sql
 ```cmd
 source /file/datad/db.sql
```
kita asumsikan db.sql berada pada folder file/datad/db.sql