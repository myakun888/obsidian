# ternary operator

terkadang kita perlu membuat kondisi sederhana , jika benar mengasilkan x, jika salah mengasilkan y

kondisi ini biasa ny kita akan mengunakan if statement, namun kita bisa persingkat dengan ternary operator


## contoh if statement

```php
$agama= "islam";

if ($agama == "islam" ){
    echo "anda adalah muslim";
    }
else {
    echo " anda adalah kafir";
}


```


## struktur thernary

```
kondisi ? true : false ;

//kondisi adalah logic nya, lalu di pisahkan dengan tanda tanya `?`
jika kondisi benar yang di amabil sebelah kiri, jika salah diambil yang sebelah kanan
```
## contoh thernary

```php
$agama = 'islam';

$agama == 'islam'? $data = 'anda adalah muslim': $data= 'anda adalah kafir';


// $data = $agama == "islam" ? " anda adalah muslim" : "anda kafir"; // ini contoh nya sama

echo $data;

//karena true maka akan menghasilkan anda adalah muslim;
```

jika di lihat hasilnya sama tapi secara baris code lebih simple