# tipeda data number (angka)

di php ada dua tipe data number yaitu **int / integer atau bulat** dan **float / bilangan pecahan**

* int
  integer bilangan bulat decimal (base 10), hexadecimal (base 16), octal (base 8), binary (base 2)
* float
  bilangan pecahan

di php kita bisa menambahakan garis bawah agar mudah di baca `_`, contoh ketika kita menulis
10000000000 (satu milyar), kita bisa menulisnya 1_000_000_000 , garis bawah ini akan di escape oleh php, ini berguna agar mudah dibaca saja

### untuk angak negatif

kita bisa menambahkan tand minus (-) minus, untuk positif tidak perlu di tambahkan,

### kita cek


disini kita menggunakan `var_dum()` adalah metod dari php yang diantaran nya berguna untuk mengecek tipe data dan juga untuk melihat nilai dari suatu variabel, jika di javascript mirip dengan metod `typeof`;

### int

contoh decimal base 10
12345

var_dump(12345)

<!-- untuk contoh yang lain silahkan lakukan hal yang sama -->

contoh decimal base oktal
01234

contoh decimal base hexadecimal
0x1234

contoh decimal base binari
0b110101

contoh underscore

1_000_000_000 ini sama dengan 1000000000(satu milyar), seperti penjelasan diatas php akan men escape tanda underscore atau garis bawah pada angka


### floating point atau pecahan
untuk pecahan di tandai dengan tanda titik `.`
contoh untuk nilai 9,5 (sembilan koma lima), di tulis `9.5`
karena php pada float membaca titik sebagai koma

contoh
1.234 ini sama dengan 1,234

contoh pada e notasi plus
1.2e3 ini sama dengan 1.2 x 1000
<!-- pada e notasi e diangap 0 (nol) angka setelahanya adalah jumlah nol nya contoh 3e2 ini adalah 300 -->

contoh pada e notasi minus
7e-2 ini sama dengan 7 x 0.01



### integer over flow

adalah suatu nilai maksimal dari php
jika sistem operasi di 32 bit maka maksimal angkanya adalah
`2147483647` dan untuk 64 bit `9223372036854775807`, jika nilai angka ny melebihi dari itu maka akan berubah menjadi floating point