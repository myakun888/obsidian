# menginstall react

untuk menginstall react ada beberapa cara
* dengan CDN (content delevery network)
* atau install di dalam project kita

menginstall di cdn kurang di rekomendasikan karena bergantung dengan internet , 

## rekomendasi install
saat kita menggunakan react, dari react itu sendiri mereokemndasikan kita untuk menginstal nya berbarengan dengan framework nya seperti
* next js
* remix js
* gatby dll


untuk menggunakan framework tersebut scope nya terlalu besar , conoth seperti next js adalah frame work full stack , sedangkan ada orang yang hanya ingin mengunakan react pada FE saja,

dari itu kita juga di rekomendasikan menggunakan tools front end, diantaranya **vite** 
(boleh kunjungi documentasi resminya)
jadi kita akan menggunakn tools ini



## setup project

pastikan pada perangkat kita telah terinstall node js


laju jalankan perintah
```cmd
npm create vite@latest
```
ini akan menginstall vite dengan versi terbaru, jika ingin versi tersendiri silahkan isi versinya

* buat nama folder project
* pilih tools nya react
* bahasa nya (disini kita contohkan dengan js)

lalu ikuti perintah berikut
```cmd
cd project_yang_kitabuattadi
npm install
npm run dev
```

setalah kita jalankan `npm install` ini menginstall semua modul yang diperlukan,
 `npm run dev` menjalan server nya

 lalu akan keluar 
 ```cmd
 http://localhost:5173
 ```
 klik atau buka link tersebut pada browser


 jika tampil anda berhasil menginstal vite