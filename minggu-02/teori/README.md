Ringkasan bab 4
#Alat Aliran Kontrol
Selain whilepernyataan yang baru saja diperkenalkan, Python menggunakan pernyataan kontrol aliran biasa yang dikenal dari bahasa lain, dengan beberapa perubahan.
#ifPernyataan
 Kata kunci ' elif' adalah kependekan dari 'else if', dan berguna untuk menghindari indentasi yang berlebihan. Sebuah if… elif… elif… urutan adalah pengganti switchatau casepernyataan yang ditemukan dalam bahasa lain.

Jika Anda membandingkan nilai yang sama dengan beberapa konstanta, atau memeriksa tipe atau atribut tertentu, Anda mungkin juga menganggap matchpernyataan itu berguna. Untuk detail lebih lanjut lihat Pernyataan kecocokan .
#forPernyataan 
Pernyataan fordalam Python sedikit berbeda dari yang biasa Anda gunakan di C atau Pascal. Daripada selalu mengulangi perkembangan aritmatika angka (seperti di Pascal), atau memberi pengguna kemampuan untuk menentukan langkah iterasi dan menghentikan kondisi (sebagai C), pernyataan Python mengulangi item dari urutan apa pun (daftar atau fora string), dalam urutan yang muncul dalam urutan. Misalnya (tidak ada permainan kata-kata)
Kode yang memodifikasi koleksi sambil mengulangi koleksi yang sama bisa jadi sulit untuk dilakukan dengan benar
#Fungsi range() _
Jika Anda perlu mengulangi urutan angka, fungsi bawaan range()akan berguna. Ini menghasilkan progresi aritmatika:
#breakdan continuePernyataan, dan elseKlausul pada Pengulangan ¶
Pernyataan break, seperti di C, keluar dari penutup foratau whileloop terdalam.
Pernyataan pengulangan mungkin memiliki elseklausa; itu dieksekusi ketika loop berakhir melalui kelelahan iterable (dengan for) atau ketika kondisi menjadi salah (dengan while), tetapi tidak ketika loop diakhiri dengan breakpernyataan
#passPernyataan 
Pernyataan itu passtidak menghasilkan apa-apa. Itu dapat digunakan ketika pernyataan diperlukan secara sintaksis tetapi program tidak memerlukan tindakan
#Mendefinisikan Fungsi 
Kata kunci memperkenalkan definisidef fungsi . Itu harus diikuti oleh nama fungsi dan daftar parameter formal yang dikurung. Pernyataan yang membentuk isi fungsi dimulai dari baris berikutnya, dan harus diberi indentasi.
Pernyataan pertama dari badan fungsi secara opsional dapat berupa string literal; literal string ini adalah string dokumentasi fungsi, atau docstring . (Selengkapnya tentang docstring dapat ditemukan di bagian Documentation Strings .) Ada alat yang menggunakan docstring untuk menghasilkan dokumentasi online atau cetak secara otomatis, atau untuk membiarkan pengguna menelusuri kode secara interaktif; merupakan praktik yang baik untuk menyertakan dokumen dalam kode yang Anda tulis
#Gaya Pengkodean
Sebagian besar bahasa dapat ditulis (atau lebih ringkas, diformat ) dalam gaya yang berbeda; beberapa lebih mudah dibaca daripada yang lain. Memudahkan orang lain untuk membaca kode Anda selalu merupakan ide yang bagus, dan mengadopsi gaya pengkodean yang bagus sangat membantu untuk itu.
Untuk Piton,PEP 8 telah muncul sebagai panduan gaya yang dipatuhi sebagian besar proyek; itu mempromosikan gaya pengkodean yang sangat mudah dibaca dan menyenangkan mata. Setiap pengembang Python harus membacanya di beberapa titik
