# operator array

di php array memiliki operator khusus , terlihat mirip tapi fungsi ny berdeda

diantaranya


| contoh        | nama           | keterangan                                                    |
| ------------- | -------------- | ------------------------------------------------------------- |
| $a + $b       | union          | berfungsi menambahkan array $a dan $b                         |
| $a == $b      | equality       | true jika $a dan $b memiliki key dan value sama               |
| $a === $b     | identity       | true jika $a dan $b memiliki key , value serta posisinya sama |
| $a != $b      | inequality     | true jika $a dan $b tidak sama                                |
| $a <> $b      | inequality<br> | true jika $a dan $b tidak sama<br>                            |
| $a !== $b<br> | noidentity     | true jika $a dan $b tidak identik                             |

### penjelesan

#### union
berfungsi menambahkan array
```php

$namaDepan = ["firstName" => "muhammad"];
$namaBelakang = ["lastName" => "fajrin"];

var_dump($namaDepan + $namaBelakang) // firstName = muhammad, lastNaem => fajrin

$namaDepan1 = [
"firstName" => "muhammad", "lastName" => "fajrin saputra"
			  ];
$namaBelakang1 = ["lastName" => "fajrin"];

// jika ada key yang sama , maka key dari array pertama yang di ambil

```
ini akan menggabungkan dua buah aray, 



#### equality

adalah `true` jika array memiliki key dan value yang sama,

```php
$namaLead = [
"firstName" => "muhammad", 
"lastName" => "fajrin saputra"
			  ];

$ceo = [
"firstName" => "muhammad", 
"lastName" => "fajrin saputra"
			  ];
var_dump($namaLead == $ceo) // true

```

#### identity

true jika memiliki key dan value serta posisi nya harus sama


adalah `true` jika array memiliki key dan value yang sama,

```php
$namaLead = [
"firstName" => "muhammad", 
"lastName" => "fajrin saputra"
			  ];

$ceo = [
"firstName" => "muhammad", 
"lastName" => "fajrin saputra"
			  ];

$namalead1 = [
"lastName" => "fajrin saputra",
"firstName" => "muhammad",
];


var_dump($namaLead === $ceo) // true
var_dump ($namaLead1 === $ceo //false, meskipun dan value nya sama, tapi posisi nya tidak sama


```

untuk operator yang lain silahkan di explore sendiri