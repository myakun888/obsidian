# component

biasa nya kita membuat tampilan itu dengan script html, berbdeda dengan react yang memiliki consep component, yang menyusun suatu ui dengan html tapi di susun dengan javasscript yang menjadi component sehingga lebih reusable

## membuat component pada react

membuat component bisa dengan cara class dan function
namun untuk saat ini react lebih merekomendasikan dengan , dan juga di dokemntasinya sudah tidak ada lagi cara dengan class

### function component

membuat component dengan function sama dengan dengan function umum pada javascript
selain itu kita juga bisa dengan arrow function

```jsx
function Tombol (){
    return (<h1> Bismillah <h1/>)
}

// atau dengan arrow function

let Tombol = ()=>{
    return (<h1> Bismillah <h1/>)
}
```

### jsx pada react

pada react kita juga memerlukan jsx yang berguna untuk menerjemahkan teks js agar dapt di baca pada html
maka dari itu file js pad react ber esktensi jsx

### membuat function component

- diawali dengan huruf kapital atau pascal case, ini bertujuan agar membedakan dengan tag pada html
- function hanya mereturn satu compoenent jadi jika kita ingin membuat component lebih dari satu kita harus membungkus nya dengan tag div kosong `<div> </div>` atau fragment teks jsx kosong `<> </>` contoh

```jsx
function Tombol() {
  return (
    <>
      <h1>bismillah </h1>
      <h1>ya rasulallah </h1>
    </>
  );
}
```

- jsx juga tidak bisa membaca teks tag <br>, jadi untuk membuat agar element ke bawah / atau di wrap bisa dengan tag `<div>`

### menambah style

pada react untuk membut style bisa dengan className , berbeda dengan html dengan nama class, ini bertujuan agar kita tau yang mana dari react dan native dari htmnl

contoh

```jsx
// pada file react
function Tombol() {
  return <button className="oke">Bismillah</button>;
}
```

file diatas memberi class dengan nama oke

```css
/* pada css */
.oke {
  back-ground: green;
}
```

dengan properti css background-color green / hijau

### perhatian

jangan pernah mendeklarasikan component di dalam component

```jsx
//  ini salah
function Tombol() {
  function Header() {}
}

// yang benar
function Tombol() {

}

function Header() {

}
```
