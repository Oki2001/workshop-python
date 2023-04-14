
Rinkasan modules
Jika Anda keluar dari juru bahasa Python dan memasukkannya lagi, definisi yang Anda buat (fungsi dan variabel) akan hilang. Oleh karena itu, jika Anda ingin menulis program yang agak panjang, lebih baik Anda menggunakan editor teks untuk menyiapkan input untuk juru bahasa dan menjalankannya dengan file tersebut sebagai input. Ini dikenal sebagai membuat skrip . Saat program Anda semakin panjang, Anda mungkin ingin membaginya menjadi beberapa file untuk pemeliharaan yang lebih mudah. Anda mungkin juga ingin menggunakan fungsi praktis yang telah Anda tulis di beberapa program tanpa menyalin definisinya ke setiap program.
Untuk mendukung ini, Python memiliki cara untuk meletakkan definisi dalam file dan menggunakannya dalam skrip atau dalam contoh interaktif dari juru bahasa. File seperti itu disebut modul ; definisi dari modul dapat diimpor ke modul lain atau ke modul utama (kumpulan variabel yang dapat Anda akses dalam skrip yang dijalankan di tingkat atas dan dalam mode kalkulator).
More on Modules
Modul dapat berisi pernyataan yang dapat dieksekusi serta definisi fungsi. Pernyataan ini dimaksudkan untuk menginisialisasi modul. Mereka dieksekusi hanya saat pertama kali nama modul ditemukan dalam pernyataan impor. 1 (Mereka juga dijalankan jika file dijalankan sebagai skrip.)
Setiap modul memiliki ruang nama pribadinya sendiri, yang digunakan sebagai ruang nama global oleh semua fungsi yang ditentukan dalam modul. Dengan demikian, pembuat modul dapat menggunakan variabel global di dalam modul tanpa khawatir tentang bentrok yang tidak disengaja dengan variabel global pengguna. Di sisi lain, jika Anda tahu apa yang Anda lakukan, Anda dapat menyentuh variabel global modul dengan notasi yang sama yang digunakan untuk merujuk ke fungsinya, modname.itemname.
Executing modules as scripts
Anda dapat menjadikan file tersebut dapat digunakan sebagai skrip dan juga sebagai modul yang dapat diimpor, karena kode yang mem-parsing baris perintah hanya berjalan jika modul dijalankan sebagai file "utama":
The Module Search Path
Saat nama modul spamdiimpor, interpreter pertama-tama akan mencari modul bawaan dengan nama tersebut. Nama modul ini tercantum dalam sys.builtin_module_names. Jika tidak ditemukan, ia akan mencari file bernama spam.pydalam daftar direktori yang diberikan oleh variabel sys.path. sys.pathdiinisialisasi dari lokasi berikut:

•	Direktori yang berisi skrip input (atau direktori saat ini ketika tidak ada file yang ditentukan).

•	PYTHONPATH(daftar nama direktori, dengan sintaks yang sama dengan variabel shellPATH).

•	Default yang bergantung pada penginstalan (berdasarkan konvensi termasuk site-packagesdirektori, ditangani oleh sitemodul).



