# switch statement


selain fitur if statement, php juga mendukung fitur swtich statement
fitur ini adalah bentuk sederhana logic dari if, yang biasa digunakan hanya untuk logica `==`

## strucktur code swtich statement

```php

$variabel = "A";

switch ($variabel){
case "A":
// code anda
break;
case "B":
// code
break;
case "C":
case "D":
// code
break;
default:
//code
}

```
## penjelasan
switch berisi acuan varibel 
case adalah nilai / kondisinya nya

break adalah akir dari satu case

default, artiya yang lainaya , atau mirip else di if statement

note , jika tidak dibatesi dengan break, contoh pada case c , d, maka case dari kedua nilai tersbut akan sama
### contoh
```php
$nilai = "A";

switch ($nilai){
case "A":
echo " nilai anda adalah $nilai , anda lulus dengan sangat baik A++";
break;
case "B":
echo "nilai anda adalah $nilai, anda lulus dengan baik";
break;
case "C":
case "D":
echo "nilai anda adalah $nilai, anda lulus";
break;
default:
echo "maaf anda belum lulus";
}
```

dilihat dari struktur nya mukin sedikit lebih panjang dari if statemnet, tetapi case ini lebih mudah dibaca,

berdasarkan code program diatas, 
* jika `nilai` berisi `"A"`, maka hasil adalah lulus dengan baik ++
* jika `nilai` berisi `"B"`, maka hasilnya adalah lulus dengan baik
* jika `nilai` berisi `c` dan `d` maka hasilanya lulus
* jika selain dari nilai diatas, `maaf anda belum lulus`;