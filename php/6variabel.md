# variabel

variabel adalah tempat untuk menampung data dan sifat nya mutable (bisa berubah)

syarat membuat variabel pada php
* diawali dengan tanda dollar `$`;
* selain nama variabel harus diawali dengan huruf atau karakter `_` underscore, selain itu tidak bisa
* bersifat ***case sensitif*** membedakan huruf besar dan kecil
* variabel dapat menampung semua tipe data diantaranya (string, int(decimal, float), arrary , object / array assosiatif dll)
### menulis variabel

```php
$nabi = 'muhammad saw';

$RASUL = 'nabi muhammad saw';

$_bersykur = 'alhamdulillah';
$jumlah_rasul = 25;

```

### variabels

fitur ini adalah menulis variabel dengan mengambil value dari variabel yang sudah ada
dengan cara menulis `$$` di ikuti dengan nama variabel nya

```php
$rasul = "muhammad saw";

$$nabi = 'rasulallah';

```

fitur ini ada tapi jarng di gunakan karena sedikit membingungkan jika di gunakan secara luas, cukup gunakan variable tidak di sarankan menggunakan fitur variables ini kecuali memang di perlukan;


## constans

* jika variable bersifat mutable(bisa berubah),jika kita inggin membuat variable yang sifat nya immutable, di php tidak ada tetapi ada fitu contasnt, 
* fitur ini jika kita buat tidak bisa berbubah lagi atau ***imutable*** cara nya 
* dengan menggunakan function define
dengan format `define("NAMA_VARIABEL",isi variable)`

```php
define("TUHAN","ALLAH SWT");
```
* best practice nya untuk memmbuat nama constant selalu gunakan huruf besar;
