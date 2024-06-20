# menginstall linux 
#linux #dualboot [[menginstall linux]]
___
menginstal linux bisa di lakukan beberapa car a
1. virtual box [[virtualbox]]
2. dualboot (berdampingan dengan os lain seperti windows dll) 
3. single boot

disini kita menginstl linux dengan cara dualboot atau berdampingan dengan os lain, dalam hal ini windows 
yang perlu di siapkan 
* file ISO os ubuntu nya 
* flasdisk untuk bootable

### Download file iso
download terlebih dahulu di situs nya plih distro atau versi sesuai yang kalian mau seperti (ubuntu, debian, mint)

### buat bootable flsdisk

selanjutnya kita buat bootble dengan flasdiks [[membuat bootable ]] kita bisa menggunakan rufus, ventoy atau sejenis nya, setelah di buat kita bisa lanjut ke prosesnya


### mebuat partisi pada windows nya

[[membuat partisi di windows]] #windows 

* masuk ke explore
* klik kanan mykomputr
* managedrive
* pilih drive yang mana mau di bagi
* dalam hal ini drive d
* sesuaikan kebutuhan untuk os linux, min 20 gb
* 
### setting bios

colokan fd ke pc / laptop, lalu nyalakn ulang
masuk ke bios dari laptop / pc kalian
untuk masuk di bios (tergantung dari laptop/pc/mobo) kalian masing masing
perhatikan petunjuk pada layar kalian pada saat di restart
biasanya tombol **f2** atau **delete** , **f12**

- setelah masuk di bios
- menju ke pengaturan booting / atau setting boot
- ubah priorty boot ke flasdisk kalain
- simpan dan restart / nyalakan ulang


### instalasi linux

#### membuat partisi
* setelah masuk ke dalam linux dengan mode live , kita bisa mencoba terlebih dahulu, atau bisa langsung kita install dengan  klik icon instalasi linux
* akan ada 3 pilihan create partisi
	* 1. instalsi berdasarkan partisi yang di create oleh linux
	* 2. instalasi mode single os, dimana ini akan menghapus bersih partisi
	* 3. instalasi berdasarkan partisi yang kita atur sendiri
	
* di contoh ini kita akan melakukan dengan mode no 3
* kita pilih partisi yang free (yang sudah kita set size nya sesuai kita buat td) **pastikan jangan salah pilih partisi, perhatikan dengan baik karena akan menformat partisi , jadi jangan salah**
* kita akan membuat partisi dan [[strucktur folder linux]], untuk dalam instalasi ini kita hanya membuat tiga partisi utama yaitu
		1. partisi root atau /
		2. partisi home
		3. partisi swap (virtual memory ny)
* setelah kita tau drive yang akan kita isi / buat partisinya , disini kita akan membuat dan menentukan size dari partisinya kita asumsikna memiliki size total 50gb
	**root** : pilih titik point root atau / , size nya buat 20gb, jenis logical / logic, format ntfs
	**swap**: (titik point tidak ada), size rekomendasi 2x total memory kita (swap tidak dbuat pun tidak masalah, jika kita memiliki memory diatas 8gb)
	**home**: titik point /home, size di min 20 gb, rekomendasi di besarkan karena semua file di simpan di sini, jenis logical / logic , format ntfs

* selajutnya next , next saja silahkan pilih sesuai yang kita mau, jika memungkinan sambungkan internet saat instalasi karena akan sekalian download
* tunggu sampai proses instalasi selesai hingga masuk halam home atau desktop nya


sampai tahap ini selesai proses intaslasi selesai,  untuk optimal adalah beberapa hal yang harus di lakukan lagi [[setelah install]] diatara nya setting user, driver dll

