Ringkasan Bab1
Jika Anda melakukan banyak pekerjaan di komputer, akhirnya Anda menemukan bahwa ada beberapa tugas yang ingin Anda otomatisasi. Misalnya, Anda mungkin ingin melakukan pencarian-dan-ganti pada sejumlah besar file teks, atau mengganti nama dan mengatur ulang sekumpulan file foto dengan cara yang rumit.seperti python ,python hanyalah bahasa untuk anda.
Python adalah bahasa yang ditafsirkan, yang dapat menghemat banyak waktu Anda selama pengembangan program karena tidak diperlukan kompilasi dan penautan. Penerjemah dapat digunakan secara interaktif, yang membuatnya mudah untuk bereksperimen dengan fitur bahasa, menulis program sekali pakai, atau menguji fungsi selama pengembangan program dari bawah ke atas. Ini juga merupakan kalkulator meja yang berguna.
Python memungkinkan program ditulis dengan kompak dan mudah dibaca. Program yang ditulis dengan Python biasanya jauh lebih pendek daripada program C, C++, atau Java yang setara, karena beberapa alasan:
-tipe data tingkat tinggi memungkinkan Anda mengekspresikan operasi kompleks dalam satu pernyataan;
-pengelompokan pernyataan dilakukan dengan lekukan alih-alih tanda kurung awal dan akhir;
-tidak diperlukan deklarasi variabel atau argumen.
Python dapat diperluas : jika Anda tahu cara memprogram dalam C, mudah untuk menambahkan fungsi atau modul bawaan baru ke juru bahasa, baik untuk melakukan operasi kritis dengan kecepatan maksimum, atau untuk menautkan program Python ke pustaka yang mungkin hanya tersedia dalam bentuk biner (seperti perpustakaan grafis khusus vendor). Setelah Anda benar-benar ketagihan, Anda dapat menautkan juru bahasa Python ke aplikasi yang ditulis dalam C dan menggunakannya sebagai ekstensi atau bahasa perintah untuk aplikasi itu.
Python mudah digunakan, tetapi ini adalah bahasa pemrograman nyata, menawarkan lebih banyak struktur dan dukungan untuk program besar daripada yang ditawarkan skrip shell atau file batch. Di sisi lain, Python juga menawarkan lebih banyak pemeriksaan kesalahan daripada C, dan, sebagai bahasa tingkat sangat tinggi , ia memiliki tipe data tingkat tinggi bawaan, seperti larik fleksibel dan kamus.
Python memungkinkan Anda membagi program Anda menjadi modul yang dapat digunakan kembali di program Python lainnya. Muncul dengan banyak koleksi modul standar yang dapat Anda gunakan sebagai dasar program Anda — atau sebagai contoh untuk mulai belajar memprogram dengan Python. Beberapa modul ini menyediakan hal-hal seperti I/O file, panggilan sistem, soket, dan bahkan antarmuka ke perangkat antarmuka pengguna grafis seperti Tk.

Ringkasan Bab2
Menggunakan Penerjemah Python
-Memanggil Penerjemah 
Penerjemah Python biasanya diinstal seperti /usr/local/bin/python3.11pada mesin yang tersedia; memasukkan /usr/local/binjalur pencarian shell Unix Anda memungkinkan untuk memulainya dengan mengetikkan perintah:

python3.11

ke cangkang. 1 Karena pilihan direktori tempat tinggal juru bahasa adalah opsi instalasi, tempat lain dimungkinkan; periksa dengan guru Python lokal atau administrator sistem Anda. (Misalnya, /usr/local/pythonadalah lokasi alternatif yang populer.)
Cara kedua untuk memulai juru bahasa adalah , yang mengeksekusi pernyataan dalam command , analog dengan opsi shell . Karena pernyataan Python sering mengandung spasi atau karakter lain yang khusus untuk shell, biasanya disarankan untuk mengutip perintah secara keseluruhan.python -c command [arg] ...-c
Beberapa modul Python juga berguna sebagai skrip. Ini dapat dipanggil menggunakan , yang mengeksekusi file sumber untuk modul seolah-olah Anda telah menyebutkan nama lengkapnya di baris perintah.python -m module [arg] ...
-Melewati Argumen 
Saat diketahui oleh juru bahasa, nama skrip dan argumen tambahan selanjutnya diubah menjadi daftar string dan ditetapkan ke variabel argvdalam sysmodul. Anda dapat mengakses daftar ini dengan menjalankan . Panjang daftar setidaknya satu; ketika tidak ada skrip dan tidak ada argumen yang diberikan, adalah string kosong.
-Modus Interaktif
Ketika perintah dibaca dari tty, interpreter dikatakan dalam mode interaktif . Dalam mode ini ia meminta perintah berikutnya dengan prompt utama , biasanya tiga tanda lebih besar dari ( >>>); untuk baris lanjutan diminta dengan prompt sekunder , secara default tiga titik ( ...). Penerjemah mencetak pesan selamat datang yang menyatakan nomor versinya dan pemberitahuan hak cipta sebelum mencetak permintaan pertama:
#Penerjemah dan Lingkungannya
-Pengkodean Kode Sumber 
Secara default, file sumber Python diperlakukan sebagai dikodekan dalam UTF-8. Dalam pengkodean itu, karakter dari sebagian besar bahasa di dunia dapat digunakan secara bersamaan dalam literal string, pengidentifikasi, dan komentar — meskipun perpustakaan standar hanya menggunakan karakter ASCII untuk pengidentifikasi, sebuah konvensi yang harus diikuti oleh kode portabel apa pun. Untuk menampilkan semua karakter ini dengan benar, editor Anda harus mengenali bahwa file tersebut adalah UTF-8, dan harus menggunakan font yang mendukung semua karakter dalam file.
Untuk mendeklarasikan penyandian selain yang default, baris komentar khusus harus ditambahkan sebagai baris pertama file
Footnotes : Di Unix, juru bahasa Python 3.x secara default tidak diinstal dengan executable bernama python, sehingga tidak bertentangan dengan executable Python 2.x yang diinstal secara bersamaan.

Ringkasan Bab3
Pengantar Informal Python
berikut, input dan output dibedakan dengan ada atau tidaknya prompt ( >>> dan … ): untuk mengulang contoh, Anda harus mengetikkan semuanya setelah prompt, saat prompt muncul; baris yang tidak dimulai dengan prompt adalah keluaran dari juru bahasa. Perhatikan bahwa prompt sekunder pada baris dengan sendirinya dalam contoh berarti Anda harus mengetikkan baris kosong; ini digunakan untuk mengakhiri perintah multi-baris.
Anda dapat mengganti tampilan petunjuk dan keluaran dengan mengeklik >>>di sudut kanan atas kotak contoh. Jika Anda menyembunyikan prompt dan output untuk contoh, Anda dapat dengan mudah menyalin dan menempelkan baris input ke juru bahasa Anda.Banyak contoh dalam manual ini, bahkan yang dimasukkan pada permintaan interaktif, menyertakan komentar.
#Menggunakan Python sebagai Kalkulator
-Angka
Penerjemah bertindak sebagai kalkulator sederhana: Anda dapat mengetikkan ekspresi dan itu akan menulis nilainya. Sintaks ekspresi langsung: operator +, -, *dan /berfungsi seperti kebanyakan bahasa lain (misalnya, Pascal atau C); tanda kurung ( ()) dapat digunakan untuk pengelompokan
-String
Selain angka, Python juga bisa memanipulasi string, yang bisa diekspresikan dalam beberapa cara. Mereka dapat diapit dengan tanda kutip tunggal ( '...') atau tanda kutip ganda ( "...") dengan hasil yang sama 2 . \dapat digunakan untuk menghindari kutipan:
-Daftar 
Python mengetahui sejumlah tipe data majemuk , yang digunakan untuk mengelompokkan nilai lain. Yang paling serbaguna adalah list , yang dapat ditulis sebagai daftar nilai (item) yang dipisahkan koma di antara tanda kurung siku. Daftar mungkin berisi item dari tipe yang berbeda, tetapi biasanya semua item memiliki tipe yang sama.
