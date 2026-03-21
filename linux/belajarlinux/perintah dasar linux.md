___
beberapa perintah dasar linux terminal, perintah ini mirip dan ada yang sama dengan terminal pada windows
beberapa perintah dasar dibagi menjadi beberapa bagian
manajemen folder , install ,cara install aplikasi di linux, user manajemen ,dan jaringan
[[cara install aplikasi di linux]], [[user management linux]]

### otamatis perintah 

saat mengtik di terminal kita bisa menggunakna otomtatis / saran yang akan di tampilkan pada terminal kita bisa menggunakan `tab`
otomatis ini penting saat kita akan mengetikan perintah `sudo apt install` pada saat kata nya sampai apt kita tekan tab maka semua saran yang mengenai apt di tampilkan, atau saat kita mengetikan kata nya tidak harus sampai selesai cukup tiga huruf contoh`sudo apt ins` lalu tekan tab, maka kata inst menjadi install, linux akan melengkapi otomatis dengan sendiri

jika fitur ini tidak aktv bisa di setting silahkan cari di online

*--help* : untuk menampilkan informasi dengan apa yang kita perlukan
contoh mengenai sudo apt
```cmd
sudo apt --help
```
maka berhubungan dengan sudo apt akan ditampilkan

*man*: menampilakan petunjuk manual lebih detail  `man katakunci`
```cmd
man sudo
```
maka semua tentang sudo akan di tampilkan penjelasannya
### manajemen folder

*dir* : untuk melihat isi dari directory,
*ls*   : mirip dengan dir yaitu menampilkan isi folder ( dapat dikombinasi dengan flag lain seperti -l, -a dan lainya)
*cd* : untuk masuk ke suatu drive
```cmd
cd namafolder
```
*mkdir* : membuat folder
```cmd
mkdir namafolder
```

*rmdir* : menghapus folder
```cmd
rmdir namfolder
```

*touch* membuat file
```cmd
touch namafile.ekstensionya
```

*cat* : melihat isi file (hanya lihat)
```cmd
cat namafile
```
*nano* : melihat isi file melalui nano teks editor bawaan linux , dapat read,write
```cmd
nano namafile
```

*vim* : melihat isi file dengan vim teks editor 
```cmd
vim namfile

``` 

*rm* : menghapus file (folder / file), disertai dengan flag ny sperti -r dll 
```cmd
rm namfolder -r

rm namfile
```
