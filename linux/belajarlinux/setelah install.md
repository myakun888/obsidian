#linux link blog luarnya  [after install linux](https://averagelinuxuser.com/ubuntu-22-04-after_install/#2-install-drivers
) [[after insall linux]]

### hal yang harus di lakukan setelah instal linux
setelah kita instalasi linux membuat login user dan password, kita harus melakukan beberapa langkah lagi agar linux lebih optimal digunakan

#### customize desktop
silahkan custome desktop sesuai kalian mau secara normal, untuk lebih explore bisa mengguanakn plguins [[gnome desktop]]

### instal driver pihak ke 3 (nvdia dll)
jika kalian menggunakan gpu external bisa lakuan ini 
buka menu >> addtional driver >>> isntal recomended propretiary driver
#### update package manager dan driver
kita akan update package manager dan driver, jalankan perintah
```cmd
sudo apt update
```
lalu masukan pass user login yang sudah kalian buat,
pada proses update ini akan mengupdate semua yang ada pada pacakge manager

#### instal preload
ini adalah aplikasi untuk agar linux lebih cepat saat membuka aplikas
jalankan perintah
```cmd
sudo apt install preload
```


#### isntal codecs dan microsoft font
ini berguna agar codec pada multimedia berjalan optimal  seperti video , audio dll dapat di gunakan di linux, juga termasuk font dari microsoft

```cmd
sudo apt install ubuntu-restricted-extras
```

#### aktifkan minimze double clik pada linux
untuk pengguna windows munkin sudah menjadi bawaan fitur ini, dimana kita jika ingin minimize hanya meklik icon aplikasi yang sedang aktv, di linux tidak seperti ini, tetapi kita bisa membuat nya bisa minimize dengan double klik dengan mengaktifkan fitur ny dengan configurasi sebagai berikut
jalan kan perintah ini pada teminal anda
[[code minimize ubuntu]] 
```cmd
gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'
```

beberapa tips diatas adalah termasuk yang penting , jika ingin lebih lengkap bisa kunjungi link ini

[after install linux](https://averagelinuxuser.com/ubuntu-22-04-after_install/#2-install-drivers
)


belajar perintah dasar linux [[perintah dasar linux]]