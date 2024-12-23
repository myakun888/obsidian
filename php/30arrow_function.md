
# arrow function

* arrow function di php di perkenalkan pada php 7
* arrow secara fungsi di gunakan untuk menggantikan anonymus function , agar di buat lebih simple
*  untuk mengakses variabel di luar closure tidak harus menggunakan kata kunci use
* pembuatan arrow function tidak menggunakan kata kunci `function` melainkan `fn`
* arrow function ini di khusus kan untuk hanya membuat function yang sederhana

```php

$doa = fn ()=>{
echo 'bismillah';
}
$doa()
// memangil variabel dari luar

$syukur = "alhamdulillah";

$doa = fn () => " hamba bersyukur ya allah $syukur ";
$doa()
```

