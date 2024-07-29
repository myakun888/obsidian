# for loop
perulangan for loop pada php

for adalah salah satu perulangan , perulangan loop pada blok code program nya akan terus diulangi selama kondisi terpenuhi atau true

### struktur kode forloop
```php
for(init;kondisi;poststatement){
    code program;
};

```
## penjelasan
* init statement, hanya akan di eksukis satu kali selama proses for loop
* kondisi, logic yang akan di cek jika benar atau true maka kode akan di jalankan, jika false maka kode tidak di jalankan
* postatement, akan di eksekusi di akhir perulangan
* note: init, kondisi, postatemnet, tidak wajib di isi, jika tidak di isi berarti nilai selalu true



### looping tanpa henti

ini adalah contoh looping tanpa henti karena, kondisi selalu true dan tidak ada counter nya

```php
for(; ; ){
    echo "alhamdulillah";
}
// ini akan looping tiada henti
```

### looping dengan kondisi

```php
{
 //contoh 1   
 $data = 0;
for (;$data <= 10;){ 

    echo "la ilahillallah $data".PHP_EOL;
$data++;
}

//contoh dua

{
 $data = 0;
for (;$data <= 10;$data++){ 

    echo "la ilahillallah $data".PHP_EOL;
}
}
}
// laillahaillah akan terus di cetak sampai jika kondisi value dari data kurang dari atau sama dengan 10;
```


### perulangan denga initstatement

```php
for($data=0;$data<=10;){

    echo "lailahaillah";
    $data++;
}


```

### perulangan denga poststatement
```php
{
    
   for ($data = 0;$data <= 10;$data++){ 
   
       echo "la ilahillallah $data".PHP_EOL;
   }
   }
```

## sintak alternatif

sintak alternatif hanya mengganti kurung kurawal
yaitu di buka dengan titik dua `:` dan diakhri dengan `endfor`;

contoh

```php
{
    
   for ($data = 0;$data <= 10;$data++): 
   
       echo "la ilahillallah $data".PHP_EOL;
   endfor;
   }
```