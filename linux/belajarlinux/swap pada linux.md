# Swap memmory

fungsi swap adalah menggantikan atau mengcover ketika memmory utama penuh,
swap terbagi menjadi dua swap file , dan swap partisi

## swap partisi
swap partisi adalah jenis swap yang dibuat di partisi, jenis swap ini di rekomendasikan

#### kelebihan
lebih aman dan jarang terjadi gagguan crash file karena telah di buat pada partisi berbeda
#### kekurangan
tidak mudah untuk di resize, karena dibuat di partisi, kita harus berhati hati takut menggangu drive lain, kita harus mengerti cara mempartisi drive 

___
untuk merize bisa mengguankan aplikasi GUI **gparted** aplikasi ini untuk menajamen partisi atau membuat partisi dengan [[membuat atau manajeman partisi dengan gparted]]


### perintah terminal swap

untuk melihat memory baik yang terpakai (memmory real atau swap) bisa dengan perintah
```cmd
free
```
ini akan menampikan memmory pada perangkat kita

menjalankan swap , disertai option dan  spec nya silahkan lihat `swapon help`,

`sudo swaponf option spec`

beberapa perintah swap
* menjalankan semua swap baik swap file atau swap partisi
```cmd
sudo swapon -a
```

* menajalankan swap dengan nama / 
```cmd
sudo swapon 
contoh
sudo swapon /dev/sda5
```
* unutk melihat rangkuman / summary pada swap 
```cmd
sudo swapon -s
```

* untuk set prioriti / prioritas pada swap
```cmd
sudo swapon -p urut namaswap 
contoh
sudo swapon -p 1 /dev/sda7
```


untuk menyetopkan
`swapoff`

kedua perintah diatas bisa disertai dengan option atau flag nya 
untuk lebih jelas silahkan liat bantuan `swapon --help` atau `swapon -help`

___
## swap file