# break dan continue


* pada materi switch case, kita sudah mengenal kata kunci break yang berguna menghentikan suatu proses case
* break juga bisa digunakan untuk menghentikan perulangan 
* case , hanya mengehentikan proses perulangan saat ini, lalu melanjutkan perulangan selanjutnya


### contoh break

```php
for($i=0;$i<=10;i$++){

    if($i==9){
        break;
    }

    echo "bismillah";
}
//ini akan mencetak hanya sampai 9
```
### penjelasan
secra logic nya 9 masih kurang dari sepuluh, dalam kondisi diatas di tambahkan kata kunci break sehingga proses perulangan berhenti


### contoh continue


```php
for($i=0;$i<=10;i$++){

    if($i==4){
        continue;
    }

    echo "bismillah";
}
//ini akan mencetak hanya sampai 10
//kecuali no 4, karena ada kata kunci continue , dimana fungsi menghentikan proses perulangan saat ini, dan melanjutkan ke perulangan selanjutnya
```