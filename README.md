- TUGAS PRAKTIKUM 2 -

- Langkah 1: Siapkan Project Baru.
  Sebelum melanjutkan praktikum, buatlah sebuah project baru Flutter dengan nama belanja dan susunan folder seperti pada gambar berikut. Penyusunan ini dimaksudkan untuk mengorganisasi kode dan widget yang lebih mudah.
  <img width="192" height="120" alt="image" src="https://github.com/user-attachments/assets/b5d1a1bf-8ccb-4c6c-b189-e5138e741972" />

- Langkah 2: Mendefinisi Route.
  Buatlah dua buah file dart dengan nama home_page.dart dan item_page.dart pada folder pages. Untuk masing-masing file, deklarasikan class HomePage pada file home_page.dart dan ItemPage pada item_page.dart. Turunkan class dari StatelessWidget. Gambaran potongan kode dapat anda lihat sebagai berikut.
  <img width="197" height="154" alt="image" src="https://github.com/user-attachments/assets/362ff7a5-323e-405d-b756-02a35731d971" />
  <img width="649" height="299" alt="image" src="https://github.com/user-attachments/assets/1bc08984-a13b-46d3-83bb-39a16caf93d8" />
  <img width="651" height="308" alt="image" src="https://github.com/user-attachments/assets/4fe5c14f-50b0-48b6-8e35-fcdfee4cf6e2" />

- Langkah 3: Lengkapi Kode di main.dart
  Setelah kedua halaman telah dibuat dan didefinisikan, bukalah file main.dart. Pada langkah ini anda akan mendefinisikan Route untuk kedua halaman tersebut. Definisi penamaan route harus bersifat unique. Halaman HomePage didefinisikan sebagai /. Dan halaman ItemPage didefinisikan sebagai /item. Untuk mendefinisikan halaman awal, anda dapat menggunakan named argument initialRoute. Gambaran tahapan ini, dapat anda lihat pada potongan kode berikut.
  <img width="657" height="346" alt="image" src="https://github.com/user-attachments/assets/22ff4e6c-06d6-471c-8c8b-6f3ce54bcce8" />
  
- Langkah 4: Membuat Data Model.
  Sebelum melakukan perpindahan halaman dari HomePage ke ItemPage, dibutuhkan proses pemodelan data. Pada desain mockup, dibutuhkan dua informasi yaitu nama dan harga. Untuk menangani hal ini, buatlah sebuah file dengan nama item.dart dan letakkan pada folder models. Pada file ini didefinisikan pemodelan data yang dibutuhkan. Ilustrasi kode yang dibutuhkan, dapat anda lihat pada potongan kode berikut.
  <img width="195" height="193" alt="image" src="https://github.com/user-attachments/assets/7930ac05-22f6-41d0-b777-3a37f7ca502c" />
  <img width="467" height="200" alt="image" src="https://github.com/user-attachments/assets/aac6b69a-72f7-4289-9bbc-e13e549452ad" />

- Langkah 5: Lengkapi Kode di class HomePage.
  Pada halaman HomePage terdapat ListView widget. Sumber data ListView diambil dari model List dari object Item. Gambaran kode yang dibutuhkan untuk melakukan definisi model dapat anda lihat sebagai berikut.
  <img width="658" height="363" alt="image" src="https://github.com/user-attachments/assets/966734e3-62c9-46b3-9b70-99b25e02a73a" />

- Langkah 6: Membuat ListView dan itemBuilder.
  Untuk menampilkan ListView pada praktikum ini digunakan itemBuilder. Data diambil dari definisi model yang telah dibuat sebelumnya. Untuk menunjukkan batas data satu dan berikutnya digunakan widget Card. Kode yang telah umum pada bagian ini tidak ditampilkan. Gambaran kode yang dibutuhkan dapat anda lihat sebagai berikut.
  

- Langkah 7: Menambahkan aksi pada ListView.
  Item pada ListView saat ini ketika ditekan masih belum memberikan aksi tertentu. Untuk menambahkan aksi pada ListView dapat digunakan widget InkWell atau GestureDetector. Perbedaan utamanya InkWell merupakan material widget yang memberikan efek ketika ditekan. Sedangkan GestureDetector bersifat umum dan bisa juga digunakan untuk gesture lain selain sentuhan. Pada praktikum ini akan digunakan widget InkWell.
  Untuk menambahkan sentuhan, letakkan cursor pada widget pembuka Card. Kemudian gunakan shortcut quick fix dari VSCode (Ctrl + . pada Windows atau Cmd + . pada MacOS). Sorot menu wrap with widget... Ubah nilai widget menjadi InkWell serta tambahkan named argument onTap yang berisi fungsi untuk berpindah ke halaman ItemPage. Ilustrasi potongan kode dapat anda lihat pada potongan berikut.
  
