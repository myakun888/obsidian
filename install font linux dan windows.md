# cara install font pada linux dan windows

#fonts #linux #windows 


## windows

- siapkan file fonts ny, silahkan donwload di situs yang ada di internet
- clik kanan file-> install
- jika font ny banyak bisa lakukan block semua lalu clik kanan ->install



### linux

ada dua cara 
1. dengan cara explore pada linux (tampilan gui) ny
2. dengan cara terminal

pada dasarnya 22 cara ini hanya memindahkan file / folder font yang ingin kita instal ke  dalam folder `/home/useranda/.local/share/fonts`




1. cara gui
	- copy file / folder font yang ingin kita install
	- lalu pastekan pada  `/home/useranda/.local/share/fonts`, biasa nya file ini tersembunyi jadi pastikan tamplikan dulu semua file nya nya
	- lalu paste kan  file / folder (font yang ingin di instal) kedalam folder font 
	- yang berada home>>local>>share>>fonts


2. cara terminal
	- copy file dengan perintah cp 
	- `sudo cp sumber pathtujuan`
	- kita asumsikan file / folder font yang ingin kita copy berada pada folder download  (kita asumsikan nama folder fontnya dengan nama jetbrain)
	- ` sudo cp pathfileanda /home/nama_useranda/.local/share/fonts`
	- contoh 
	- `sudo cp jetbrains /home/dianwisora/.local/share/fonts`
note : dari contoah kita asumsikan folder jetbrains berada di dalam folder downloads, ini berlaku relatif path


> jadi inti dari cara install font di linux , yaitu hanya memidahkan font/ folder fonts yang kita ingin instal ke dalam folder fonts yang beradan di share
	- `home/useranda/.local/share/fonts`