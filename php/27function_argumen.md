# function argumen

setelah kita bisa membuat function, kita juga tau bagaimana cara memangilnya


* perlu kita ketahui function juga bisa memangil argument, kita bisa mengirim informasi ke function yang ingin kita panggil

* untuk melakukan tersebut kita perlu menggunakan argument
* cara membuat argument sama seperti membuat variabel
* argument di tempatkan di dalam kurung function tersebut
* argument bisa lebih dari satu, jika lebih dari satu di pisahkan dengan tanda koma `,`


```php
//membuat function argument


function doa ($doaAnda){

    echo "bismillah saya ingin $doaAnda";
};

doa("kaya raya"); // bismillah saya ingin kaya raya
doa("seluruh keluarga besar berjumpa dengan rasulallah saw di surga")

```
nilai atau value nya akan berisi sesuai dengan apa yang kita isi kan pada argument nya
dalam contoh di ataas adalah `kaya raya`


## default argument value

pada function juga mendukung default argument value, artinya jika kita tidak mengisi argument, maka nilai default nya akan mengisi nya

```php
function asmaulHusna ($namaallah = 'ALLAH SWT'){
    echo "salah satu nama allah $namaAllah";

};

asmaulHusna ("ya malik"); // ini ya malik
asmaulHusna (); // ini ALLAH SWT
```

### kesalahan dalam menggunakan default value

saat kita mengunakan argument lebih dari satu, jika kita ingin mengunakan default value, posisikan default value jangan pada argument / parameter pertama, karena akan tidak berguna

```php
function name ($firstname= 'anonymus', $lastname){

echo "nama lengkap $firsnamr $lastname";
}

name("testing"); // ini error , karena ini mengisi argumen pertama, yang kedua tidak di isi, sedangkan default value nya ada di argument pertama,
```
## type declaration

di php argument mirip variabel, tipe data nya dinamis, selain dinamis kita juga bisa menentukan tipe data dari suatu variabel, misalnya nya kita ingin tipe argument nya kita khususkan int, string dll, di argument bisa kita lakukan 

berikut valid type pada argument


| Type              | keterangan                                                   |
| ----------------- | ------------------------------------------------------------ |
| class / interface | parameter harus tipe class / interface                       |
| self              | parameter harus sama dengan class dimana function ini dibuat |
| array             | parameter harus array                                        |
| callable          | parameter harus callable                                     |
| bool              | parameter harus boolean                                      |
| float             | parameter harus float                                        |
| int               | parameter harus integer                                      |
| string            | parameter harus string                                       |
| iterable          | parameter harus iterable                                     |
| object            | parameter harus object                                       |

### contoh penggunaan tipe deklarasi pada argument function

```php

function data (int $nilai, int $nilai2){
$total = $nilai + $nialai2;

echo "hasil dari penjumlahan $nilai + $nilai2 = $total"

}


data(1,8)
data("1","88")
data(true,false)
data([],[]) // error
```
pada contoh diatas tipe deklasrari juga mampu menconversi contoh jika kita menseting argument ke tipe int, jika kita memasukan angka string maka php otomatis mengconversi ke angka int, tapi jika teks tidak bisa
begitu juga jika bool, karena boolean true adalah 1, dan false adalah 0, ini bisa di conversi
untuk yang tidak bisa di conversi akan error

## variabel length argument list

pada argumen juga kita bisa membuat argumen atau parameter yang yang mampu menampung banyak nilai
ini jika di `javascript` di namakan `rest parameter`

di php di namakan `variabel-lenght argument list`

cara menggunakanya cukup tambahkan notasi titik 3. di depan argumentya
nilai yang di kembalikan berupa tipe data array 

```php
function data(...$nilai){
forEach($nilai as $value){
echo $value;
}
}


data(11,12);

