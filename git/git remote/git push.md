# Git Push
___
saat melakukan perubahan pada code kita , perbuhan hanya terjadi secar local , belum termasuk pada repository online kita (github/gitlab), agar perbuhan tadi dapat di online kan kita harus melakukan *push* 
cara melakukan push 
`git push nama_remote namabranch_remote`

itu adalah perintah nya , jika di remote belum ada otamatis akan dibuatkan sama dengan nama brach di local . contoh

```git
git push origin master
```
artinya git push ke remote orgin dan nama branch_remote nya adalah master, maka di branch master ini akan ad comit dari local tadi ,
jadi perintah ini secara otomatis juga akan menbuat branch (jika di remotenya tidak ada branch yang di maksud)

