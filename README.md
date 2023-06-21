### Saya Muhammad Yusuf Bahtiar NIM 2107980 mengerjakan Latihan Praktikum 12 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

<br>

## Deskripsi Tugas

Keterangan :

- Bagi yang hadir pada saat praktikum, jelaskan perbedaan struktur di LP yang sebelumnya telah dikerjakan dengan struktur file TMD.
- Bagi yang tidak hadir, jelaskan struktur file TMD yang sudah dikerjakan (MVP / MVVM), dan mengapa menggunakan struktur itu.

<br>

## Penjelasan

Struktur file/framework yang saya gunakan pada Tugas Masa Depan (TMD) yang telah saya kerjakan adalah **MVVM**, yakni Model, View, dan View Model. Dengan keterangan sebagai berikut :

1. Model
   - Box
   - DB 
   - GameInterface
   - GameObject
   - Player
   - ScoreTable
2. View
   - Display
   - Menu
3. View Model
   - Controller
   - Game
   - Handler
   - Music
   - Processing

Di mana proses bisnis pertama kali dimulai dengan pengaksesan terhadap *class* `Menu` melalui *class* `Main` (tidak dimasukkan ke dalam folder manapun, karena keinginan pembuat soal TMD), sebagai salah satu *class* di folder View, pada *class* `Menu` tersebut akan melakukan proses pengaksesan data melalui *class* `Processing` yang ada di folder View Model, yang nantinya akan dilanjutkan untuk me-*request* data ke *score table* yang ada pada *database* melalui *class* `ScoreTable` dan *class* `DB` di folder Model. Data yang telah didapatkannya akan dikirimkan kembali ke *class* `Processing`, untuk kemudian ditampilkan oleh *class* `Menu` ke layar. Selain itu, dilakukan juga pemrosesan musik oleh *class* `Menu` melalui *class* `Music`.

Saat pengguna memulai *game*-nya proses yang terjadi adalah pembuatan *display* dengan *class* `Display`, yang nantinya akan digunakan untuk menampilkan *game*-nya. Jadi setelah membuat *display* akan dilakukan pembuatan *game* melalui *class* `Game`, pada saat akan memulai *game* akan banyak proses yang terjadi seperti pembuatan *controller* melalui *class* `Controller`, pembuatan *handler* melalui *class* `Handler`, serta pembuatan setiap objek yang ada (Player dan Box) dengan yang bertugas untuk itu ialah *class* pada folder Model seperti `Box`, `GameInterface`, `GameObject`, dan `Player`. Setelah proses pembuatan dilakukan, hasilnya akan diatur oleh setiap *class* yang ada di folder View Model untuk nantinya ditampilkan oleh *class* di folder View.

<br>

Alasan menggunakan struktur **MVVM** : 

MVVM dipilih sebagai arsitektur pada Tugas Masa Depan ini karena dapat memisahkan tampilan dan proses bisnis dengan baik, serta lebih fleksibel sehingga setiap statenya dapat dikelola dengan baik. Selain itu, dengan digunakannya MVVM pada Tugas Masa Depan ini dapat memberikan kemudahan terkait pemeliharaan dan melakukan proses pengembangan yang lebih efisien jika kedepannya ingin dilakukan pengembangan terkait Tugas Masa Depan ini.
