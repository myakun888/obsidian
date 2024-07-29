# vpn

apa itu vpn, vpn adalah singkatan dari **virtual private network** 
dimana profile internet kita akan di samarkan


setup vpn pada linux dan windows

pastikan kita memiliki akun vpn, kita bisa singup atau login ,
rekomendasi akun ny bisa dari **protonvpn dan zoogvpn**




## setup vpn
berdasarkan setup bisa di bagi menjadi 2 bagian 
1. insttal applikasi nya
2. secara manual config di jaringan nya


untuk cara 1, cukup mudah kita tinggal download apliksi 

di contoh ini kita akan menggunakan cara 2, config secara manual, karena secara manual ini lebih powerful dan efisien


## linux

contoh dengan proton vpn dan zoogvpn

### proton vpn

1. login dan masuk ke akun prootonvpn
2. pada menu unduhan, donwload sertifikat dari salah satu negara server yang di berikan secara free


3. pastikan install `network-manager-openvpn-gnome`
   cara nya ` sudo apt-get install network-manager-openvpn-gnome`

4. jika sudah di install masuk ke configurasi jaringan pada linux
   dengan cara, pengaturan >> jaringan >> vpn >> + (tambah) >>> pilih impor dari berkas
   pilih file yang sudah anda download td
5. pilih identitas / identiti
6. masukan user name dan password dari vpn, (note) untuk protonvpn kalian harus buka akun, karena tidak sama dengan akun login nya, silahkan buka akun liat di profile / akun nya, akan ada `nama pengguna open vpn` dan `passowrd ny`
7. copy kedua nya dan masukan pada config yang tersedia lalu save



### zoog vpn

hampir sama dengan proton , pastikan kita sudah login dawnload file config / certifikan nya , biasanya zoog ini memberi file config yang isi nya certifikat crt dan file servernya 
untuk server gratis (usa, inggris, belanda)
untuk severs nya biasanya diberi dua jenis (udp, tcp) rekomendasi gunakan udp

lanjut setting pada linux ny

pastikan sudah install network manager openvpn gnome

1. masuk ke configurasi jaringan pada linux
   dengan cara, pengaturan >> jaringan >> vpn >> + (tambah) >>> pilih impor dari berkas
2. masukan sertifkan crt nya dan file servernya (rekomendasi gunakan yang udp)   
3. masukan username dan password akun zoog nya
