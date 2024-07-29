# function
* function adalah block program yang akan di eksekusi ketika di panggil

* function di tandai dengan tanda ()
function terbagi menjadi dua function bawaan / built in dan function kita buat sendiri

* function bawaan diantaranya 
isset(), count() dll

* pada bahasa pemrograman lain funciton juga di sebut method

## mebuat function
membuat function cukup gunakan kata kunci `function` nama dan tand (), dan diakhiri dengan {}

strukturnya adalah sebagai berikut
```php
function nama () {
//code program
}
```

contoh
```php
function doa (){
    echo "bismillah";
}

//ini namanya adalah function doa
```

memanggil function yaitu namanya dan diikuti dengan ()
```php
doa ()

// memangil function doa
```

## lokasi function
* php sangat flexible dalam membuat funciton
* pada php kita bisa membuat function dimanapun
* tidak seperti bahas pemrograman lain harus ada aturan tertentu
* kita bisa membuat di dalam if atau di dalam funciton lagi
* untuk menjalankan function harus di panggil agar kode nya berjalan

### contoh lain function

```php
$data = 'bismillah';

if($doa=='bismillah'){
    function doa(){
        echo "alhamdulillah";
    };
}

doa()

```