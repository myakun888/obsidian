# cara setting path pada linux dan windows


seting envirotment biasanya di gunakan agar kita dapat mengakses suatu aplikasi dari terminal dan megekseskusi nya secara global melalui terminal


## cari alamat yang ingin di simpan

contoh kita ingin menyimpan alamat php
pada windows biasanya terdapat pada data:c /program file / bin

pastikan kita tahu path dari bin suatu app yang ingin kita tambahkan di evnirotment
copy path nya  lalu masukan di envirotment ny

berikut cara memasuki envirotmen / setting envirotment pada windwos dan linuex
## windows

*  `ctr + r`
* lalu ketik `env` atau `envirotment` lalu enter
* pilih edit path
* new
* lalu masukan alamat path yang ingin kita tambahkan

## linux

pada linux
 ada dua cara 
1. setelah kita tahu alamt path nya contoh alamat path php berada pada 
	`/opt/lampp/bin` 
	pastikan kita berada pada path lokasi yang ingin kita copy
	lalu ketik `cp php /bin`
	(ini berlaku relatif path atau absolut path)

2. cara kedua, pastikan kita berada pada path `home` ketik `ls -a`
	 cari file dengan nama `.bashrc` atau `.profile` , untuk ubuntu biasanya di `.bashrc`
	 lalu buka dengan code editor kalian bisa dengan nano atau vscode atau lainya
	 di contoh ini dengan vscode , lakukan perintah berikut
	ketik `code .profile`
	tambahkan  perintah berikut dengan formant `export = pathnya :$PATH`
	contoh
	`export = /opt/lampp/bin:$PATH`
	save dan buka ulang terminal

inti dari dua cara ini yaitu meletakan lokasi file bin ke env ny

silahkan gunakan dua cara diatas , biasanya cara ke 2 gunakan, untuk cara pertama itu secara root karena di pindkan ke bin dari root , sedangkan cara dua adalah ke bin user melalui envirotment user 
	 