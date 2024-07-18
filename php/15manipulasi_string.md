# manipulasi string

string adalah tipe data text, string kita bisa maksimalkan dengan memanipulasinya jika diperlukan

### dot (.) / titik

dot (.) adalah operator yang digunakan untuk mengabungkan string dengan tipe data lain , selain dot bisa juga dengan plus (+) tapi ini tidak di rekomendasikan karena akan error jika digunakan dengan tipe data int / number / floating point


```php
$data= 'bismillah';

echo ($data.'ya allah'.php_EOL);
echo ('ya allah ya tuhanku'. "allah swt");

```
***note : `php_eol` (end of line) pengganti enter atau `"\n"` ***


### konversi string
diantara manipulasi lainya terdapat juga konversi string ke number (int, flot) dan sebaliknya
dengan function bawaan dari php

```PHP


$konversiString = string(100);
$konversiNumber = number("100");
$konversiFloat = number("100.1");

//menhasilkan susai angka nya

var_dump($konversiString); //"100"
var_dump($konversiNumber); //100
var_dump($konversiFloat); //100.1


// bagaimana kalau tidak sesuai? maka nilai yang akan di kembalikan no 0
//contoh kita akan mengconversi string text ke angka

$teks = number("testing");
var_dump($teks) // 0
```



### mengakses karakter
selain manipulasi tersebut, di php string juga dapat kita akses karakter nya mirip seperti array dengan menggunakan index nya
index pertama adalah 0


```php
$data = 'bismillah';

echo($data[0]).PHP_EOL;// b 
echo($data[1]).PHP_EOL;// i 
echo($data[2]).PHP_EOL;// s 
echo($data[3]).PHP_EOL;// m 
echo($data[4]).PHP_EOL;// i 
echo($data[5]).PHP_EOL;// l 
echo($data[6]).PHP_EOL;// l
echo($data[7]).PHP_EOL;// a
echo($data[8]).PHP_EOL;// h

```

### variabel parsing

pada php kita bisa mengakses nilai / value dari suatu variabel ini bisa di gunakan jika kita menggunakan kutip dua `"` atau herodeoc , lalu gunakan tanda  `$` (dollar)

fungsi nya agar memudahkan kita menggabungkan value dari variabel dengan string 

ini juga di sebut interpolasi pada bahas pemrograman javascript

```php

$doa = 'bismillah';

echo "selalu baca $doa dalam setiap mengawali aktivitasmu " // selalu baca bismillah dalam setiap mengawali akttivitasmu
```

### culry brace / kurung kurawal { }

kadang kita ingin menambahkan atau menggabungakn teks tanpa ada jeda seperti 
atau tanpa spasi , ini tidak bisa di lakukan oleh double quote / kutip dua, 
baik dengan dot (.) pun tidak bisa
untung nya ada curly brace atau kurung kurawal bisa

contoh
```php
$teman = 'friends'

//ini tanpa kurung kurawal
echo ("hallo $teman s  "); // ini akan menjadi " hallo friend s " 


//ini dengan kurung kurawal
echo ("hallo {$teman}s "); // ini menjadi " hallo friends "
```

