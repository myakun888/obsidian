
# Git branch
#gitbranch
branch ada cabang , jadi di git secara default memiliki cabang utama yaitu master / main
tetapi kita juga bisa menambah / atau membuat cabang branch
### membuat branch dengan git

```git
git branch namabranch
```

### membuat branch dan langsung (checkout ke branch tersebut)

```git
git checkout -b namabranch
```
### menghapus branch
untuk menghapus branch kita bisa menggunakan flag `-d` atau `--delete`
```git
git branch -d namabranch
```

### menampilkan semua branch
```git
git branch 
```
ini akan menampilkan semua branch, dan yang di beri tanda bintang / asteric itu adalah di mana branch aktiv saat ini

untuk lebih banyak info branch bisa di lihat di help 
dengan perintah
```git
git branch -help
```
atau
```git
git branch --help
```
### branch pada remote
[[git remote branch]]

## mengbungkan hasil commit dari branch lain

untuk mengabungkan commit dari branch lain, ada banyak cara dan kondisi diantaranya
[[merge]], [[git rebase]], [[git cherrypick]] dll