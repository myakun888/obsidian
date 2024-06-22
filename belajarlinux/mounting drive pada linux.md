# Mounting Drive / disk pada linux


## cara mount drive manual

bagi pengguna windows, selain drive C, drive yang terpisah akan tetap terbuka seperti drive d dll, berbeda dengan linux, untuk mengakses drive lain kita harus meklik nya agar terbuka / di kaitkan terlebih dahulu agar bisa diakses oleh user

terkadang drive yang sudah di  buat tidak bisa di akses , agar bisa di akses kita harus me **mounting** manual berikut caranya

* buat folder untuk tempat kita menampung file dari drivenya
* lalu jalankan perintah 
* `sudo mount -m path_drive_yang_ingin_dbuka lokasi_folder_untuk_membukanya`

contoh
kita memiliki drive yang tidak terbuka otomatis , kita asumsikan alamatnya 
**/dev/sda5** , setelah mengetahui drive nya (drive ini yang akan kita buka) , lalu kita buat juga folder yang bebas taro dimana , ini digunakan untuk menampung isi dari drive nya kita asumsikan foldernya **datafile** (data ini path nya /home/user/documendatafile)

```cmd
sudo mount -m /dev/sda5 /home/user/documen/datafile
```


### cara melepaskan drive / unmount

untuk melepaskan cukup jalankan perintah `sudo umount path_drivenya` dalam hal ini **/dev/sda5** atau `sudo umount path_folder_penampungnya`

```cmd
sudo umount /dev/sda5
```

atau dengan path penampungnya **datafile** yang berdada pada path absolutnya /home/user/documen/datafile
```cmd
sudo umount /home/user/documen/datafile
```



## mounting flasdisk / cd atau media lainya

untuk flasdisk cd atau media lainya , jika tidak tampil pada berkas , tetapi kondisinya terhubung kalian coba cek di folder media pada usernya
karena folder media adalah tempat untuk memount file pihak ketiga sperti usb, cdrom dll

jika tidak bisa dibuka dengan klik , kita harus me lakukan mounting manual , caranya sama , dengan diatas

```cmd
sudo mount -m /media/namuser folder_untuk_membukanya
```