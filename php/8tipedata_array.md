# array

* array adalah tipe data kosong, atau banyak data
* array dapat menampung banyak tipe data, diantaranya **string, int, null dll**

* array memiliki panjang dinamis artinya kita bisa menmabah array tampa batas

## membuat array

array mirip map pada bahas pemrograman lain 
ada beberapa cara membuat array pada php sintaks ny sebagai berikut
ada yang memiliki key dan value, dan ada yang tidak 

1. cara pertama , ini memiliki key dan value;
` array ( key => value,
 key => 'value', )

 cotoh
 ```php
 $data = array (
    'nabi' =>"ya rasulallah saw",
    'agama' => "islam",
    'ke'=> 25,
    1=> 'terbaik');


//cara dua dengan shorthand ny

$data2 =[
    "rasul"=>'rasulallah saw',
    "kitab" => 'alquran'
];


 ```
dari dua cara diatas itu cara membuat array tinggal kita pilih

kalau di perhatikan array ini lebih tepat nya di sebut array assosiatif karena memiliki key dan value (mirip oject pada javascript)

### array tanpa key 

```php
$agama = ['islam','krinten','hindu','buda']
```

ini juga di sebut 
tinggal kita pilih sesuai kebutuhan


### beberapa operasi array

* mengambil nilai array berdasarkan index `$array[indexnya]` contoh `$agama[0]`

* mengubah nilai array berdasar index nya dan memberi value baru
 `$array[index]= 'value'`

* menambah array , dari posisi belakang `$array[]= value`
  
* menghapus data array dari index, index ny juga terhapus
  `unset($array[index])`

* menghitung panjang array
  `count($array)` 


### array di dalam array / array multi dimensi
karena array dapat menampung data secara dinamis array pun dapat menampung array lagi atau di sebut array multi dimensi

```php
$nabi = [
    ['muhammad saw','isa as','daud as'],
    ['islam','kristen','yahudi']
];


$rasul= [
    "nama" => "ya rasullallah saw",
    "mukjizat" =>[
        1=> "kitab suci alquran",
        2=> "memberi syafaat ke umat nya",
        3=> "dapat membelah bulan"],
    "gelar" => "SAW"  
];
```

kalau sekilas array assosiatif ini mirip object pada javascript;