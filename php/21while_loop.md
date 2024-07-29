# while loop

adalah bentuk sederhana dari for loop
dimana hanya ada kondisi saja tidak ada inistatement dan poststatement

## struktur code while loop
```php
$data=0;

while(kondisi){

$data++
}

```
di dalam tanda kurung hanya ada kondisi, tidak ada init dan post statement

contoh

```php
{
    $data = 0;
    while($data<=100){
        echo "alhamdulillah";
    };

   }

```

## sintak alternatif

untuk sintak altenatif nya
sama nya hanya menggangi kurung kurawal, untuk pembuka dengan tanda titik dua `:` dan di akhri dengan `endwhile`;

```php
{
    $data = 0;
    while($data<=100):
        echo "alhamdulillah";
    endwhile;

   }
```