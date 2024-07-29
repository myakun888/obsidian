-# if statement

sebelum memasuki materi if statement kita bahas dikit tentang percabangan

## percabangan atau control flow

adalah suatu logika di dalam pemrograman di mana apabila ada suatu syarat yang terpenuhi atau true maka akan ada aksi di eksekusi



di bahas pemrograman sudah umum memiliki control flow 
termasuk if stament di php

struktuk nya


```php
if(kondisi){
//eksekusi code program disini
}
```

```php
$tuhan = "allah";

if($tuhan == "allah"){
echo "benar tuhan kita hanya $tuhan";
}
// benar tuhan kita hanya allah
```

pada code program diatas jika variabel tuhan benar berisi allah
maka akan di cetak "tiada tuhan selain allah"
jika tidak maka tidak tampil apa apa , karena tidak ada kondisi else / kondisi lain


### else
else adalah kondisi lain atau kondisi false dari suatu statement jika kondisi true tidak terpeuhi

struktur ny

```php
if(kondisi){
//eksekusi code program disini
}else{
//eksekusi code program disini
}
```

contoh code program

```php
$kitabsuciUmatIslam = " ";

if($kitaSuciUmatIslam == "alqran" ){
echo("benar kitab suci umat islam adalah alquran");
}
else {
echo("itu bukan kitab suci umat islam")
}

//jika kondisi salah maka yang akan di tampilkan adalah block kode program else
```


### else if

jika if hanya satu kondisi terkadang kita menggunakan lebih dari satu kondisi maka kita harus menggunakan `else if` atau `elif`
else if ini berguna jika kita membuat if staement lebih dari satu kondisi

```php

if(kondisi1){
//code program
}
else if (kondisi2){
//code program
}
else if (kondisi3){
//code program
}

else {

}
```

contoh kode program
```php

$nilai = 80

if($nilai >= 75){
echo "nilai anda A"
}else if ($nilai >=60){
echo "nilia anda b"
}else if ($nilai >=30){
echo "nilai anda c"
}else{
echo "nilai anda d"
}

```


### sintax alternatif

pada if statement kita juga bisa menggunakan sintax alternatif pengganti kurung kurawal `{ }` yaitu tand a`:` titik dua dan diakhri dengan 'endif'
fungsi nya sama saja

silahkan di pilih salah satu

struktur nya
```php
if(kondisi):
//eksekusi code program disini
endif
```

contoh
```php
$tuhan = "allah";

if($tuhan == "allah"): // tanda kurung kuruwal diganti titik dua :
echo "benar tuhan kita hanya $tuhan";
endif // di tutup dengan endif
```
