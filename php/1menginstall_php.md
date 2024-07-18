# Menginstall PHP

mengistall php bisa kita unduh melalui website pribadinya , tapi terdapat kesulitan karena kita harus mengconfig secar manual dan memerlukan compiler dari c++

dianjurkan kita menginstal php dari paket bundler seperti **XAMPP, LAMPP** dll, karena dari bundler tersebut sudah tergabung diantaranya servernya, dan semua hal yang di perlukan seperti mysql/mariadb, apache, httpd dan termasuk php itu sendiri

di sini kita menggunakan **XAMPP**

jadi saat kita menginstall xampp secara otomatis kita mendapatkna semua paket tersebut



## seting path

setelah di install xampp kita perlu setting path, karena kita ingin munggunakan php dari terminal (agar bisa di akses dari terminal)

setiap os memiliki cara yang berbeda untuk setting path tp memiliki inti sama yaitu mengcopy lokasi bin dari suatu file

* windows: 
  cari folder bin dari php ( setealah tau copy path nya) , tergantung dimana kita menginstall nya , biasanya berdada pada data:c /fileprogram
  lalu buka atau tekan `windows + r` ketikan 'env' 
  lalu edit path dan tambahkan lokasi path yang sudah ti copy tadi


* Linux

di linux ada dua cara
1. dalam hal ini contoh kita menginstal xampp
buka atau ketikan `cd /opt/lampp/bin` 
lalu copy file php dan tarok pada root bin , dengan cara
`sudo cp php /bin`
atau 
`sudo cp php ../../../bin` 
silahkan dicoba saya yang mana berlaku path relatif atau absolute

lalu lakukan juga pada mysql nya
`sudo cp mysql /bin` dan seterusnya

cara 1 adalah inti nya mengcopy file bin suatu aplikasi ke bin rot

2. cara dua
  buka file (.bashrc atau .profile) biasanya di file .bashrc , pada home linux
  file ini tersembunyi jadi gunakan ls -a
tambakan script

`export= lokasi file bin: $PATH` 
contoh 
file bin php ada pada lokasi /opt/lampp/bin , maka ketikan 

`export=/opt/lampp/bin:$PATH`
setelah itu buka ulang terminal nya

dan jalankan testing nya
## testing

untuk memastikan jika setting path sudah benar coba jalankan perintah pada terminal
`php --version` 
jika tampil versi dari php nya maka seting path berhasil


dalam materi ini kita belum mengunakan server xampp karena kita hanya menjalankan pada terminal, sedangkan xampp di gunakan saat proses pada website