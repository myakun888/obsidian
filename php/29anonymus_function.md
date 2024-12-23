
# anonymus function

* pada php juga terdapat anonymus function
* anonymus function adalah function yang tidak memiliki nama
* function ini biasanya digunakan untuk jadi argument, atau sebagai value variabel
* anonymus function membuat kita bisa mengirim function sebagai argumen



```php


$doa = function (){
echo 'bismillah';
}
$doa()
```


## anonymus function sebagai argumen

pada contoh ini kita menggunakan function anonymus sebagai argumen,

```php

function berdoa ($nilai, $data2){

$hasil = $data2($nilai);
echo $hasil;
}

berdoa('bismillah',function($nilai){
return strtoupper($nilai)
});
```

### mengkases variabel di luar closure

secara default anonymus function hanya dapat mengakses variabel di dalam closure nya, tetapi kita dapat mengakses keluar dengan mengunakan kata kunci `use`

pada contoh ini kita akan mengaskes variabel di luar closure nya
```php
$nabi = 'NABI MUHAMMAD SAW';

$sholawat = function () use ($nabi){
echo "$nabi"
}

$sholawat(); // NABI MUHAMMAD SAW
```