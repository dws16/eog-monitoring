# EOG Monitoring

Sebuah website untuk monitoring data EOG ~~yang dibuat khusus untuk Lutfi Ananditya Septiandi~~

## Struktur Folder

```
├───controllers
├───db
│ ├───migrations
│ └───models
├───public
│ ├───model
│ └───socket.io
├───routes
└───views
```

## Proses Instalasi

1. Buat database dengan nama `eog_monitoring`
2. Jalankan command `npm i` untuk install seluruh _package_ yg diperlukan
3. Jalankan command `npm run migrate` untuk membuat table yg sudah ditentukan di folder `db/migrations/*js`
4. Jalankan command `npm run dev` untuk menjalankan website

## Fitur

- Menampilkan grafik EOG yg diambil dari database dengan mengakses url `http://localhost:3001/`
- Insert data dengan url `http://localhost:3001/data/` menggunakan method `POST` dengan contoh body:

```
{
  "time": 10
  "data": 30.78
}
```
