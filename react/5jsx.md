# menulis markup di javascirpt
jsx adalah extensi untuk javascript agar kita dapat membaca tag html, atau dengan kata lain untuk dapat menulis html di javascript kita memerlukan jsx


web dibangun dengan 3 core utama yaitu HTML, CSS dan JAVASCRIPT ,
dulu dibuat terpisah dimana hmtl di html dan logic di javascript
dan keduanya ini terpisah

semakin perkembangan web, memungkinkan kita dapat membuat logic dan markup dalam satu file , dengan javascript dan react comoponent
dimna react dengan component class dan function component


### menconver markup kedalam javascript

contoh saat kita membuat markup

```html
// html
<h1>bimsillah</h1>
<p>ini adalah html biasa</p>
```
```jsx
function Doa (){
    return (
        <>
        <h1>bismilla</h1>
        <p>ini contoh function component</p>
        </>
    )

}

```

## aturan dalam menulis di jsx

1. mengembalikan single element
jsx pada react dalam comoponent hanya bisa mengembalikan satu atau single element
contoh

```jsx
function Doa (){
    return (<p>bismillah</p>)
}
```
jika ingin lebih dari satu element maka wajib di bungkus dengan tag `<div> </div>` kosong atau tag kosong `<> </>`
ini juga di sebut fragment pada jsx

```jsx
function Doa (){
    return (
        <div>
        <p>bismillah</p>)
        </div>
}
```

2. tutup semua tag
pada jsx kita wajib menutup semua tag atau harus ada close tag , meskipun itu single tag contoh seperti tag `image, br, hr `

contoh

```html
<!-- jika di html hanya seperti ini -->
 <img src='xxx' alt='xx'>
```

tapi di jsx wajib di ada close tag 
```jsx

<img> </img>
//atuah
 <img src="sumberdll" alt='xxx' />  </>


```

3. penggunan cammelCase 
pada jsx teknik penulisan cammelcase wajib digunakan dalam menulis attribut / props (properti) , dan yang lain
contoh
pada penulisan class pad hmtl kita cukup menulis `class`
tapi pada jsx kita harus menulis ny `className` ini agar membedakan class ini adalah dari jsx
, dan penulisan atribut jika pada html menggunakan tanda min (-) jika dua kata, tapi jsx menggunakan teknk cammelCase
```jsx
<img className="data" />


```


## javascript jsx dengan kurung kurawal { }

dengan jsx memunkinkan kita menulis markup html di dalam javascript file, serta merender logic dan menampilkan file di satu tempat yang sama

terkadang kita ingin menambahkan sedikit logic di dalam html atau mengamil value dll, disini fungsi kurung kurawal dapat  digunakan untuk melakukan itu
<!-- kurung kurawal { } untuk membuka , memfungsikan javascript di dalamnya -->
jika di file javascript biasa kita bisa menggunakan tanda backtik dan ` ` dan `${}`
di jsc cukup dengan `{}` saja


contoh


```jsx
function Data (){
    let nama = 'rasulallah saw`
    return (
        <>
        <h1> {nama} </h1>
        <>
    )
}


```

### dimana harus menggunakan kurung kurawal
1. langsung di dalam sebuah jsx tag contoh 
   
```jsx
function Rasul (){
   
   let rasul = 'rasulallah saw';
   return (
    <>
   <h1> rasul saya adalah {rasul}  </h1>
   </>
   )
   // ini akan menampilkan rasul saya adalah rasulallah
        }
   ``` 
 2. sebagai atribut  
   contoh kita akan mengambil nilai dari suatu variabel unutk di masukan ke dalam atribut, untuk memasukan nya kita cukum menambahkan tanda `=` dan `{}`

```jsx
   let 
   function Gambar () {
let url = 'gambar.jpg`
   return (
    <image src={url} />
   )
   }
  // ini akan mengahasilkan url = 'gambar.jpg' 
   ```

### menggunakan double kurung kurawal {{}}

kita juga bisa menyisipkan object dengan menggunakan double kurung kurawal pada jsx, contoh saat kita ingin menysisipkan style secara inline (cara ini kurang baik, tetapi ini hanya, cara yang terbaik untuk styling tetap gunakan className)

```jsx
let desain ={
    backgroundColor: 'green';
    teks: 'white';
}
<img className='oke' style= {{desain}} />

//atau
<img className='oke' style= {{backgroundColor:'blue',teks:'white'}} />

```
karena react tidak mendukung untuk menulis secara embeded, tetapi bisa di dilakukan dengan cara object