# Git Semantic commit

#git #semantic_commit
semantic commit atau convensional commit adalah suatu teknik menulis commit pada git 

berikut formant nya
``` cmd
<type>(scope):<subject> 
```
`scope` hanya optional

``` cmd
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in present tense.
|
+-------> Type: chore, docs, feat, fix, refactor, style, or test.
```




### contoh

```cmd
feat : menambahkan fitur jumlah
```


atau dengan scope
- `feat(data.js): menambahkan fitur jumlah`


diawali dengan type nya , lalu boleh ditambahkan dengan scope(cakupan nya) , lalu di ikuti dengan keterangan nya

contoh kedua dengan scope

`style(header): menambah bootstap`


jadi ini inti dari semantic / convensional commit adalah memberikan keterangan yang jelas , testruktur dan desktriptip serta mudah di pahami

> perlu di ingat
> setiap type bisa berbeda beda tergantung dari kita atau kesepakan dari team / perusahan saat berkolaborasi

berikut berbagai  type dan artinya

* `feat` = mendesripsikan ke pada feature baru bagi user
* `fix` = untuk bug fix
* `docs` = merujuk pada documen
* `style` = merujuk pada style , formating dll , tidak ada perubahan pada production code
* `refactor` = untuk refactoring, baik penamaan variabel dll ( tidak ada perubahan pada production code)
* `test` = menambahkan testing
* `grunk` = update task grunk dan lainlain

refrensi dari [git semantic code](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)

silahkan juga baca **conventional commmit**  untuk informasi lainya