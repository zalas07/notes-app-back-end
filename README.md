# Notes App Backend
## Requirement yang harus di selesaikan
**Notes App Backend** merupakan sebuah proyek *Restfull API* yang harus di selesaikan oleh setiap peserta yang tergabung dalam modul **Backend with Google Cloud** di Dicoding Academy Platform.
adapun beberapa kriteria yang perlu di perhatikan dalam pengerjaan aplikasi *backend* ini terdiri dari beberapa persyaratan seperti di jelaskan pada masing- masing point di bawah ini:
> Di kutip dari Dicoding Academy Platform
1.  aplikasi yang di buat harus menggunakan port **9000**. tetapi jika komputer tidak mensupport port 9000, maka buatlah dengan port lain, tetapi ketika submission hendak di kirim, silahkan ganti dengan port **9000**
2.  aplikasi yang di buat harus memiliki runner script. cara membuatnya dapat menggunakan properti *start* kedalam properti script ***package.json*** sebagai berikut:
   `{
    "name": "submission",
    ...
           "scripts": {
             "start": "node src/server.js",
           }
         }'

3. ***API*** dapat menyimpan buku melalui *route*
   - method : **POST**
   - URL : **/books**
   - Body Request : {
    `"name": string,
    "year": number,
    "author": string,
    "summary": string,
    "publisher": string,
    "pageCount": number,
    "readPage": number,
    "reading": boolean
}`
4. **API** dapat menampilkan seluruh buku
   - method :**GET**
   - URL : **/books**
     server harus mengembalikan response dengan:
   -status code : **Berhasil**
5 **API** dapat menampilkan detail buku yang di simpan melalui routes
- method :**GET**
- URL :**/books/{booksid}**
6. **API** dapat mengubah data buku berdasarkan *ID* melalui *Route*:
  -method : **PUT**
  -URL : **/books/{bookId}**
7. **API** dapat menghapus buku berdasarkan *ID* melalui route berikut:
  -method : **DELETE**
  URL : **/books/{bookid}**
## Testing / Pengujian
Ketika membangun *Bookshelf API*, tentu kita perlu menguji untuk memastikan API berjalan sesuai dengan kriteria yang ada. Dicoding telah menyediakan berkas Postman Collection dan Environment yang dapat di gunakan gunakan untuk pengujian:
[postman Bookshelf API test Collection](https://github.com/dicodingacademy/a261-backend-pemula-labs/raw/099-shared-files/BookshelfAPITestCollectionAndEnvironment.zip)



