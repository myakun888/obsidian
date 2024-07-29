# foreach

saat kita menggunakan tipe data array, kita bisa mengeluarkan isi nya denga menggunakan forloop
tetapi itu kurang efisien, akan leih baik kita menggunakan fucntion/ method khusus untuk array yaitu forech()


## perulangan tanpa foreach

ini contoh hanya dengan for

```php
$rasul = ['MUHAMMAD SAW','IBRAHIM AS', 'ISA AS','ISMAIL AS', 'DAUD AS'];


for($i=0;$i<count($rasul);$i++){
    echo "$rasul[$i]".PHP_EOL;
    //ini hanya dengan looping
};

```

### sruktur foreach

```php

foreach($array as $x){

//code


}
//ada dua parameter pertama array nya , kedua mendiskripsikan value nya
```
## perulangn dengan foreach

```php

foreach($rasul as $value){
    echo "$value".PHP_EOL;
};

```


### foreach dengan key dan value

foreach juga bisa digunakan untuk aray yang memiliki key dan value atau array assosiatif

```php

foreach($rasul as $key => $value){
    echo "$key = $value".PHP_EOL;
};
// memiliki 3 parameter
// pertama arraynya
//kedua key nya
//ke tiag value nya
```