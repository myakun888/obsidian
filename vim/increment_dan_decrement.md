# Increment dan Decrement 

#vim #vim_tips
Increment adalah *MENAIKAN / MENAMBAHKAN* nilai satu tingkat 
Decrement adalah *MENURUNKAN / MENGURANGI* nilai satu tingkat



fitur ini akan berjalan hanya pada tipe nilai integer / angka 


contoh 
tulis angka berapapun lalu posisi kan cursor diatas angka nya dan 
tekan 
`ctrl + a` -> untuk Increment
ctrl + x -> untuk Decrement
```vim 

1 

```
```
```




## membuat list nomor / list number


kita dapat memanfaatkan Increment dan Decrement untuk membuat list number 

cara nya 
ketik jumlah baris kebawah 
bisa di awali dengan nol

> O (huruf O besar) membuat baris baru ke atas
> o (huru o), membuat baris baru ke kebawah 

langkah nya sebagai berikut 

`jumlah_baris o ` `formatny contoh 0.` lalu `tekan tombol Esc`
`setelah itu blok semua , lalu g ctrl+a` -> untuk incremeent
`ctrl + x ` -> untuk decreement


contoh kita akan mebuat 5 baris ke bawah
1. `5.o`  -> enter
2. `0.` 
3. tekan ESC
4. blok semua baris
5. tekan `g` -> enter
6. `ctrl + a`  (untuk incremeent/ `ctrl+x` untuk decreement)



```vim
1.
2.
3.

```

