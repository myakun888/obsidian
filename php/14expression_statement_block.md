# Expression, statement dan block



ini hanya sekedar pengetahuan untuk kita

### expressi
expressi dalam php adalah suatu variabel yang memimiliki nilai
contoh

```php

$data = 5;  // ini expression

$data_A = $data; 


function doa ()
{
return echo "bismillah" ;
}

$bismillah = doa(); 

//jika suatu memiliki nilai itu dianggap expressi, (variabel,array dll) meskipun null
```



### statement
adalah kumpulan dari beberapa expresi dan diakhiri dengan tanda titik koma `;`

```php
$data = 5;

$data_A = $data;

function doa ()
{
return echo "bismillah" ;
}

$bismillah = doa(); 
```


### block
adalah kumpulan  statement atau nol statement yang berada di dalam kurung kurawal `{}`

```php

{
echo "bismillah";
echo "bismillah";
echo "bismillah";
}
```