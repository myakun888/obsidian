# tipe data string

tipe data string adalah tipeda yang mereprsentasikan teks
untuk menulis teks diawali dengan tanda kutip dua `"`, atau dengan kutip satu `'`

## kutip satu / single quote '
contoh
```php
echo ' bismillah ';
``` 

## kutip dua / double quote
kelebihan double quote kita bisa memasukan escape karaketer seperti `\n` untuk enter dan juga bisa untuk interpolasi yaitu membaca variabel
```php
echo " bismillah"
```

```php
$nabi= 'muhammad saw';

echo " nabi ku adalah $nabi \n aku bersaksi ${nabi} utusan allah

```
<!-- untuk interpolasi bisa dengan ${nama_variabel} atau $nama_variabel, cara dengan kurung kurawal sudah tidak di rekomendasikan lagi di php 8 keatas-->
itu akan mengahasilkan 
" nabi ku adalah nabi muhammad saw
aku bersaksi nabi muhammad utusan allah "


## multiline string
kadang kita ingin menambahkan string yang panjang dan memiliki lebih dari satu baris
kita sebenarnya bisa menambakan escape karakter yang berperan sebagai enter `\n`
tetapi php memiliki fitur yang lebih baik dimana jika kita ingin membuat string panjang dan banyak baris kita tidak perlu menggunakan `\n`
yaitu dengan fitur php bernama `Heredoc` dan `Nowdoc`;

 contoh heredoc

 ```php
 echo <<<mfs
 bismillah hirohmanirohim 
 ini adalah contoh string panjang

 mfs
 
 ```

 conoth nowdoc
secara fungsi hampir mirip dengan herodoc tetapi nowdoc tidak memiliki fungsi parsing seperti herodoc, 
materi parsing akan di bahas pada materi manipulasi string
 ```php
echo<<<'mfs'
 bismillah hirohmanirohim 
 ini adalah contoh string panjang
mfs
```