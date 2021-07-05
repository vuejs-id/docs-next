# Pedoman Gaya Dokumentasi

Panduan ini akan memberikan gambaran umum tentang berbagai elemen desain yang tersedia untuk Anda gunakan dalam membuat dokumentasi.

## Peringatan (*Alerts*)

VuePress menyediakan sebuah plugin wadah khusus untuk membuat kotak peringatan. Ada empat jenis: 

- **Info**: Memberikan informasi yang netral
- **Tip**: Memberikan informasi yang bersifat positif dan menganjurkan sesuatu
- **Warning**: Memberikan informasi yang harus diperhatikan pengguna karena ada risiko tingkat rendah hingga sedang
- **Danger**: Memberikan informasi yang bersifat negatif dan memiliki risiko tinggi terhadap pengguna

**Contoh Markdown**

```
::: info
Anda dapat menemukan informasi lebih lanjut di situs ini.
:::

::: tip
Ini adalah tips yang bagus untuk diingat!
:::

::: warning
Ini adalah sesuatu yang harus diwaspadai
:::

::: danger
Ini adalah sesuatu yang tidak kami rekomendasikan. Gunakan dengan risiko yang Anda tanggung sendiri.
:::
```

**Markdown yang Dirender**

::: info
Anda dapat menemukan informasi lebih lanjut di situs ini.
:::

::: tip
Ini adalah tips yang bagus untuk diingat!
:::

::: warning
Ini adalah sesuatu yang harus diwaspadai
:::

::: danger
Ini adalah sesuatu yang tidak kami rekomendasikan. Gunakan dengan risiko yang Anda tanggung sendiri.
:::

## Blok Kode

VuePress menggunakan Prism untuk memberikan penyorotan sintaksis bahasa dengan menambahkan nama bahasa ke backtick (`) di awal blok kode:

**Contoh Markdown**

````
```js
export default {
  name: 'MyComponent'
}
```
````

**Keluaran yang Dirender**

```js
export default {
  name: 'MyComponent'
}
```

### Penyorotan Baris

Untuk menambahkan penyorotan baris ke blok kode Anda, Anda perlu menambahkan nomor baris dalam kurung kurawal.

#### Baris Tunggal

**Contoh Markdown**

````
```js{2}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
````

**Markdown yang Dirender**

```js{2}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```

#### Sekumpulan Baris

````
```js{4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
````

```js{4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```

#### Beberapa Bagian

````
```js{2,4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
````

```js{2,4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
