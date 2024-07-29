# do while loop

adalah suatu perulangan mirip dengan while perbedaanya hanya dalam kondisi, jika perulangan lain seperti for, while, dll , selalu melakukan pengecekan kondisi di awal lalu di lanjutkan dengan eksekusi programan,
sedangkan `do while` melakukan eksekusi terlebih dahulu baru melakukan pengecekan kodnisi

sehingga do while akan selalu minimal 1x melakukan eksekusi code programan meskipun kondisi logica tidak terpenuhi

## struktur kode do while

```php
$nilai = 0;
do{
    echo 'alhamdulillah';
$nilai++;
}while($nilai > 0);
```

### penjelasan
pada code diatas, value dari nilai adalah 0, dan kondisi ny jika $nilai > dari 0;

tetapi untuk do while , kode program meskipun kondisi salah / false, kode minimal akan di eksekusi satu kali, karena alur nya ekseskui dahulu baru di cek kondisinya;