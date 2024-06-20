# Membuat Remote pada git / git remote

#gitremote 
## membuat remote
setelah kita membuat dan melakukan perubahn pada local, mungkin kita akan membagikan / mempublish / mengupload atau untuk melakukan kerja team agar repositori kita bisa di gukan oleh team lain

untuk melakukan itu kita harus membuat remote agar bisa menghubungakn repo local kita dengan yang di github/gitlab

* pastikan kita sudah ada / sudah membuat reposistory di github/gitlab atau sejenis nya 
* jika sudah dibuat , copy link nya (ssh/ httpnya), lalu jalankan perintah berikut
`git add remote namaremote linkrepositorynya` contoh
```git
git add remote origin http/www.nabimuhamamdsaw
```

artinya kita membuat remote dengan nama remote **origin**, untuk link repositry **http/www.nabimuhamamdsaw**


## melihat remote

untuk melihat remote kita bisa menggunakan perintah
```git
git remote
```
untuk melihat lebih detail, remote nya link nya kemana
```git 
git remote -v

atau

git remote --verbose
```

## mengubah nama remote
```git
git remote rename namaremotelama namaremote baru

```

## untuk menghapus
 ```git
 git remote remove namaremote
```

untuk lebih banyak perintah git remote silahkan cek di `git remote -help ` atau `git remote --help`