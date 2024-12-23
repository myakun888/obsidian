
# variabel function

* pada php ada fitur variabel function, artinya dimana kita bisa memanggil function dari sebuah value yang terdapat dari variabel
* untuk memanggil variabel function kita cukup memangil nama variabel ny contoh $namaVariabel(), jika ada argument kita bisa gunakan argument $namaVariabel(argument)


```php
// function nya

function doa (){
echo "bismillah";
}

function doa2 (){
echo "bismillah bismillah";

}

//variabel

$pangilDoa = 'doa' // nama function nya kita buat jadi string sesuai dengan nama functionnya
$pangilDoa2 = 'doa'
// kita gunaka fuction doa , ini cara manggilnya
$pangilDoa();
$pangilDoa2();

```

### menggunakan argument untuk variabel function

```php

function sayHello ($name,$filter)}

$nama = $filter($name)
echo "nama sudah di ubah $nama"
}

sayHello("Bisimllah","strtoupper")
sayHello("Bisimllah","strtolower")

```