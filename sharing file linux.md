# sharing file linux

#linux 
saring file pada linux sangat mudah, terbagi menjadi dua cara 
dengan cara 
- gui (tampilan)
- dengan aplikasi samba

note: pastikan windows nya sudah si setting network ny bisa diakses


### cari gui

cara ini di gunakan jika kita ingin mengakses file yang sudah di share oleh komputer lain, dan kita masuk melalui jaringan yang sama / dalam hal ini komputer tujuan kita adalah windows


kita asumsikan alamat ip dari komputer tujuan adalah 192.688.100.8
1.  buka / klik folder berkas
2. perhatikan di seblah kiri, klik `+ lokasi lain`; (berada pada sisi kiri bawah)
3.  liat di tengah bawah , masukan protok dan alamat ip ny
	alamat protcol , silahkan pilih biasanya
		1.  `//nfs:` ---> network file sistem
		2. `//smb:`---> aplikasi samba (bila belum instal silahkan isntal)
4. masukan protcol dan alamat nya
 `//protocl:alamatip`	contoh kita menggunakna samba
	//smb:192.168.100.8
5. lalu enter, masukan passwrod  / buat password jika di minta

contoh diatas cara sharing file, dimana kita mengakses file yang di share dari komputer lain



## dengan samba

samba adalah salah satu aplikasi yang di gunakan untuk melakukan sharing file dari linux

jika belum instal silahkan instal  `sudo apt install samba`;

kita asumsikan ip dari komputer linux ini
`192.168.100.88`;

cara ini adalah kita yang akan bertindak berbagi / share , contoh kita akan membagikan / sharing file dari komputer kita dengan nama foler / file 
`file_berbagi` jadi komputer lain bisa mengakses file kita


1. pastikan kita sudah membuat file yang ingin kita sharing
	kita juga bisa buat dari cmd, kita asumsikan kita berada di home( sebenarya bebas)
	`mkdir sharing`        // ini untuk membuat foler
	`chmod 777 sharing`    // kita mengubah permision agar  full akses foldernya
2.  lanjut kita melakukan configurasi di aplikasi samba, di file config ny
	kita ke file config nya berada pada path  `/etc/samba/smb.conf`
3.  buat user name untuk login file ny dan password ketikan , ini akan kita masukan saat mengakses file yang di sharing tadi
	```cmd
	useradd datasaring  // dalam contoh ini kita buat datasaring
	smbpasswd -a datasaring (enter) // isi paswword yang kita inginkan
	```
4. lalu buka file config nya dengan code editor anda  bisa dengan cara
	`code /etc/samba/smb.conf`
	lalu kita setting script nya
```cmd
	[data file]   // ini adalah nama yang akan di tampilkan di jaringan

	comment = isi komentra // boleh dibuat atau tidak
	valid user = nama_user yang dibuat td //ini nama user yang kita buat untuk folder tadi
	path    =              // laksi path folder / file yang ingin di share
	browseable = yes        //agar bisa di akses dari browsing
	writeable = yes/no // yes berati bisa kita tulis file ny	

```

**note**
jika tidak ingin membuat password  pada file yang kita sharing
lewati langkah ke 3, 
lalu tidak perlu di tulis / hapus baris properti 
`valid user`


### mengakses nya
jika kita ingin mengakses dari windows

buka explorer data nya, ketik ip linux os yang melakukan sharing file tadi 
pada bar path explorer windows




untuk lebih lanjut silahkan liaht dokumentasi samba
atau bisa liat di youte cara sharing file dari linux ke windows


