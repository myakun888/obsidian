# export path di linux



saat kita menggunakan linux kita biasa nya menjalankan file biasanya file executable atau bin , atau berbentuk app.image dll melalui terminal, terkadang ada kendala di mana file bin nya hanya bisa di eksekusi di tempat nya saja, maka dari itu agar bisa di eksekusi di semua tempat harus kita export, tarok di bin seperti cara berikut ini


## ada beberapa cara export path di linux  

## 1. dengan export PATH

kita export di path ny di file `.bashrc`  


file ini berada di home file linux   tersembunyi  , jadi lihat dengan `ll -a`  

- buka file `.bashrc ` dengan code editor  
- tambahkan `export "path ny:$PATH"`  
contoh 

```bahsrc
export "/opt/lampp/bin:$PATH"
```

ini bearti kita mengexport semua file bin yang ada pada `opt/lampp/bin`, sehingga bisa di akses dari mana saja 

buka ulang terminal jalankan file bin nya
dalam contoh ini kita ingin menjalankan file bin php.bin, karena file bin php.bin tersimpan di  lampp

`php --version`
jika berhasil akan tampil versi dari php yang di install di dalam file lampp nya



## 2  local bin

kita juga bisa dengan menempatkan file exceutebale nya di local `usr/local/bin` atau di `usr/bin`


cara nya cukup copy atau memindahkan file excutbale nya id file bin ( `boleh di /usr/local/bin `   atau `/usr/bin`)  


## 3 membuat symbolic link

ini hampir mirip seperti cara ke dua 

tapi kita tidak mengcopy atau memindahkan file bin nya  melainkan kita membuat nya terkoneksi atau tersambung atau link  , kedalam file `/usr/local/bin` atau `/usr/bin`

dengan cara  dengan perintah `ln -s pathlokasifile pathlokasi/namabaru`  

contoh kita memiliki file bin di folder `/home/data/php.bin`

kita buat terkoneksi dengan tujuan file ny ke `/usr/local/bin`

note pastikan path nya absolut ke file exutable nya / bin nya  

contoh  
`ln -s /home/data/php.bin /usr/local/bin/php`  

sekarang sudah terkoneksi silahkan liaht menggunakan `ll` makan akan ada file dengan nama
`php  >> /home/data/php.bin `

ini menandakan sudah terkoneksi , kita bisa menjalankan file php di cmd di mana saja  

untuk mengahpus nya cukup hapus nama  file link nya saja , dalam hal ini php  


note perlu di ingat , karena ini saling terkoneksi pastikan file asli nya jangan di hapus karena jika hilang atau terhapus tidak akan berjalan  