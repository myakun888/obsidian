# operator logika

operator yang bertugas memmbandingkan dua nilai boolean dan merturn boolean lagi



| operator   | nama | hasil                                                   |
| ---------- | ---- | ------------------------------------------------------- |
| $a && $b   | and  | jika a dan b keduanya true , maka hasilnya true         |
| $a and $b  | and  | jika a dan b keduanya true , maka hasilnya true         |
| $a \|\| $b | or   | jika salah satu nya true (a tau b), maka hasilnya true  |
| $a or $b   | or   | jika salah satu nya true (a atau b), maka hasilnya true |
| !=$a       | not  | true jika nilai a adalah false                          |
| $a xor $b  | xor  | true jika salah satunya true, tapi tidak keduanya       |
dari nama diatas terdapat yang sama diantranya `and  or `
kita bisa pilih salah satu misalnya untuk operator `and` itu sama dnegan `&&` hanya kode nya saja berbeda



contoh pada operator logia


```php

var_dum(true && true ); // menghasilkan true
var_dum(true || false ); // menghasilka true
```