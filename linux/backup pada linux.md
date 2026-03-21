# Backup linux

#linux 

untuk membackup linux kita memerlukan aplikasi yang bernama
**timeshift*

`sudo apt install timesift`\


setelah di intasll ada beberapa configurasi

1. type akan ada pilihan `rsync` dan `btrfs`, secar default akan di pilih rsync
2. location, pilih drive mana yang akan di backup
3. jadwal di sini ada mulai dari, `bulan minggu hari jam dan boot`
	 disini ada pilihan pertahankan, maksud nya adalah ketika kita memilihih pilihan perthankan 2, maka ketika backup terjadwal berlaan file sudah ada tiga , maka hanya dua yang tetap disimpan, (1 yang paling lama akan di hapus, dua yang terbaru akan di pertahankan
4. user, akan ada pilihan user dan root, disini ada ceklist / radio type jenis file apa yang akan di cadangkan
		- kecualikan semua file, artinya hanya menyimpan sistem  ( ini rekomendasi)
		- sertakan file tersembuny, artinya file sistem dan file tersembunyi akan disimpan
		- sertakan semuanyan artinya semua file di simpan


### membackup

untuk membackup tinggal pilih tombol `buat` atau `create` maka akan otomatis dibuat sesui dengan configurasi diawal, 

pada proses ini sistem timesift akan memperkirakan berapa jumlah file / ukuran file yang akan di backup

jika sudah selesai makan akan tampil list hasil back up yang kalian lakukan 


### merestore

pilih backupan pada list yang ingin kalian restore dengan cara di klik , lalu tekan `restore`

### menghapus resotore
klik file file restore yang ingin di hapus lalu klik `delete`


### jelajahi
tombol ini sama sperti browse mencari file backup yang mungkin anda simpan pada lokasi / drive lain



## lokasi penyimpanan

lokasi pemyimpanan awal saat kita melakukan backup pada timesift biasanya berada pada folder  `/home` dengan nama file folder **timesift**
ini adalah contoh ketika menyimpan untuk file home 


jadi kita bisa menyimpan hasil backupan dengan mengcopy file ny ke drive lain

