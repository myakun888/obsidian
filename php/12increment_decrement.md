# increment dan dercement
 
php juga mendukung gaya pemrograman C++, yaitu increment dan decrement
   
## increment

adalah menaikan data number sebanyak 1 angka

dari jenisnya terbagi dua
yaitu post (sesudah) dan pre (sebelum)

  ## decrement

adalah menurunkan data number sebanyak 1 angka
dari jenisnya juga terbagi dua yait post dan pre

  
### tabel increment dan decrement (post dan pre)





| contoh  | nama           | efek                                                            |
| ------- | -------------- | --------------------------------------------------------------- |
| $data++ | post increment | kembalikan nilai $data, lalu naikan satu tingkat / tambah satu; |
| ++$data | pre increment  | naiknan satu tingkan dan kembalikan nilai $data                 |
| $data-- | post decrement | kembalikan nilai $data, lalu turunkan satu tingkat              |
| --$data | pre decrement  | turunkan satu tingkat, lalu kembalikan nilai $data              |


```php

$data = 10;

var_dum($data++)
```