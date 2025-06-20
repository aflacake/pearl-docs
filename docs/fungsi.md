# `fungsi`
`fungsi` digunakan untuk membuat **fungsi sendiri** di Earl. Fungsi ini bisa dipanggil berkali-kali dengan parameter yang berbeda, seperti bahasa pemrograman pada umumnya.

## Format Penulisan
```earl
fungsi namaFungsi(param1, param2)
(
   -- isi kode fungsi ---
)
```
- Gunakan `(` dan `)` dibaris terpisah sebagai pembuka dan penutup blok fungsi
- Gunakan kembalikan nilai untuk mengembalikan hasil dari fungsi

## Contoh Fungsi Menyapa
```earl
fungsi halo(nama)
(
  tampilkan "Halo, " nama
)
```
Pemanggilan:
```earl
Halo "Dunia"
```
Keluaran:
```bash
Halo, Dunia
```

## Contoh Fungsi Kembalikan
```earl
fungsi tambah(a, b)
(
  kembalikan a + b
)
```
Eksekusi:
```earl
evaluasi tambah 5 4
```
Keluaran:
```bash
9
```

Aturan penting
- Nama fungsi hanya boleh terdiri dari huruf, angka, dan `_`, dan tidak boleh diawali dengan angka.
- Parameter dipisahkan dengan koma: (x, y, z).
- Harus menggunakan tanda kurung `(` dan `)` untuk membungkus isi fungsi.
- Fungsi disimpan sebagai modul sementara dan bisa langsung dipanggil setelah didefiniskan.

Tips
- Simpan fungsi umum seperti `tambah`, `kalikan`, `format` dalam file `.pearl` dan impor jika dibutuhkan.
- Gunakan `kembalikan` untuk menghentikan fungsi lebih awal dan memberi hasil.
