# tipe data null

null adalah tipe data tapi tidak ada nilai;
saat kita membuat variabel tapi kita ingin menghapus data tidak dengan variabel nya nya kita bisa membuat nilai nya menjadi null,
contoh

```php
$data = null; // ini lebih baik
$data0; // dari pada ini, karena ini bisa undifined
```

null kita bisa gunakan jika variabel yang tidak memiliki data

unutk membuat data null cukup masukan tesk `null` atau `NULL` incasesensitfi contoh

```php
$data= null;
//atau
$data2 = NULL;
```

## mengecek apakah data null
selain dengan var_dump yang memang berguna untuk mengecek semua variabel, phpjuga memilik funciton kusus yaitu is_null
untuk mengecek kita bisa gunakan function `is_null()`
jika kita langsung `var_dump()` dia akan meruturn isi datanya
jika menggunakan `is_null()` akan merteturn boolean
```php
$data = null;

echo is_null($data) // jika null mereturn 1, jika false tidak mereturn atau 0

var_dump(is_null($data)) // ini merertunr boolean , jika true maka null, jika false tidak null

// atau

$isnull = is_null($data)
var_dump($isnull);
```


### mengahapus variabel

jika kita ingin benar benar menghapus variabel, dan juga datanya
kita bisa menggunakan function `unset()`, tapi berhati hati menggunakan ini, karena akan menghapus dan tidak menggap ada variabel yang sudah di deklrasikan, bahkan null pun tidak terbaca, hasil nya akan diangap undifined
 
 contoh;

 ```php
 $data = 'kebaikan';

 unset($data);

 echo $data; // ini akan undifined , karena telah di hapus dengan unset()
 
 ```


### untuk mengecek apakah variabel itu ada nilainya atau null;

jika function `is_null()` adalah mengecek apakah suatu variabel itu `null` atau `tidak`

`isset` adalah function yang berguna mengecek apakah suatu variabel ada nilainya atau tidak / null

hampir mirip dengan is_null

return dari isset jika ada nilai maka mereturn angka boolean 1 jika true, kosong / 0 / tidak ada apapun adalah false

```php
$info = 'ada';
$noinfo= 'null';

echo "$info"; // 1 atau true;
echo "$noinfo"; // kosong atau false;

```
