
# Git remote branch

lanjutan dari branch lokal [[git branch]] #gitremote
[[membuat remote]]

### melihat branch

melihat branch remote 
```git
git branch -r
```

melihat semua branch baik di lokal dan di remote

```git
git branch -a
```
untuk mendapatkan dengan cara  berikut
## membuat / menambahkan branch dari remote branch

1. saat kita melakukan clone kita hanya mendapatkan remote branch master / main nya saja untuk branch yang lain tidak dapat
jika kita ingin membuat branch dan mengabil commit nya juga berikut cara nya


```git
git checkout -b namalokalbranch namaremote/remotebranch
```
contoh nama nama remot nya origin, nama branch remote nya fitur1
maka, untuk nama  (note: kita belum membuat nama branch1)
```git
git checkout -b branch1 origin/fitur1
```
perintah diatas adalah membuat branch dengan nama branch1 sekaligus mengambil semua isi dari branch remote origin dengan isi branch yang diambil adalah branch fitur1

2. jika kita sudah memiliki branch dan kita ingin mengisi branch tersebut dengan remote branch dari branch remote carany adalah sebagai berikut
```git

git pull namaremote namabranch
```

contoh kita sudah memiliki branch lokal dengan nama branch2, pastikan kita berada pada branch tesrbut lalu kita tarik / donwload branch remote yang kita ingin kan

```git
git pull origin fitur1
```
cara kedua ini juga bisa dengan pull,
untuk lebih detail mengenai pull akan ada dimateri [[git pull ]] dan [[git push]]



### menghapus branch remote

sama hal nya dengan saat membuat , jika kita hanya menghapus remote branch pada local, remote pada branch belom terhapus, untuk menghapus ny adalah
`git push -d namaremote namaremotebranch`

```git
git push -d origin fitur2
```
dalam hal ini nama branch ny adalah origin, dan nama remote branch yang dihapus adalah fitur2

