# Joint

adalah menggabungkan data dari dua tabel atau lebih,

join dapat di guanakan tanpa contraint , tapi baiknya di kombinasikan dengan constraint

joint ada beberapa macam

1. inner join
2. lefft join
3. right join

## 1. inner join

cara join nya

contoh kita ada 2 tabel

**Barang**

| id  | nama     |
| --- | -------- |
| 1   | laptop   |
| 2   | mouse    |
| 3   | ssd      |
| 4   | keyboard |
| 5   | usb      |
| 6   | monitor  |

**transaksi**

| id  | jumlah | id_barang |
| --- | ------ | --------- |
| 1   | 55     | 1         |
| 2   | 10     | 3         |
| 3   | 5      | 6         |

```sql

select barang.nama, transaksi.jumlah from barang inner join on barang.id = transaksi.id_barang

```

| nama    | jumlah |
| ------- | ------ |
| laptop  | 55     |
| monitor | 5      |
| ssd     | 10     |

nama itu dari tabel barang, dan jumlah dari tabel transaksi

untuk yang tidak ada id nya maka tidak di tampilkan pada innerjoin

## 2. left join
