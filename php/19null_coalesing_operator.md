# null coalesing operator

operator ini berguna untuk mengecek jika suatu variaberl bernilai null isi nya kita ganti dengan yang kita ingginkan, tetapi jika tidak null tampilkan nilai sesui isinya


sebenrya kita bisa menggunakan dengan if statement
contoh

```php
// $data = []; // ini kita buat null
$data = ["bismillah"];
$cek = isset($data[0]);

if( $cek ){
    $hasil = $data[0];
}
else{
    $hasil = "data kosong";
}

echo $data;
```
contoh diatas dengan statement if
jika data null maka di tampilkan `data kosong`, jika tidak null atau ada isi datanya maka tampilkan `isi datanya`



## menggunakan null coalesing

```php

$data = ['bismillah'];
$hasil =  $data[0]?? "tidak ada data";

echo $hasil;

```

dari contoh diatas jika jika data memiliki nilai, maka value dari hasil sama dengan data, jika data nilainya null, maka isi hasil adalah tidak ada data