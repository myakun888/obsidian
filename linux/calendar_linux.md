# calendar

perintah calendar linux pada cmd / terminal

kita bisa menggunakan `cal` dan `ncal`
perintah kedua nya mirip nya hanya beberapa perbedaan sedikit

dan juga ada parmeter dan falg ny 


## cal

### melihat calendar
untuk melihat kita bisa menggunakan perinta
`cal`
ini akan menampilkan calendar bulan saat ini

### melihat beberapa bulan kedapan
`cal -A3`
ini akan menampilkan bulan saat ini dan dua bulan kedepan

### meliha 3 bulan
`cal -3`
ini akan menampilkan 3 bulan, bulan saat ini, 1 bulan kebelekang dan 1 bulan kedepan

### melihat beberapa bulan kedepan
`cal -B3`
ini akan menapilkan  bulan saat ini dan 2 bulan kebelakang

### melihat tahun
`cal tahunnya`
contoh `cal 2024` 
ini akan menampilkan tahun 2024

### melihat bulan
`cal bulanya`
contoh `cal mar`
ini akan menampilkan bulan maret
jika ingin disertakan tahunya , tambahkan saja tahunya

## ncal

ncal adalah aplikasi dari pacakge apt, jadi kita harus menginstall nya dahulu untuk dapat menggunakannya
`sudo apt install ncal`

### beberapa perintahnya

ncal ini mirip dengan call, perintahnya baik dari parameter atau flag nya
perbedaan nya jika menggunakan ncal, akan manampilkan hari / tanggal saat ini

contoh
`ncal maret 2024'
akan manampilkan maret 2024 dan hari saat command ini di akses;


