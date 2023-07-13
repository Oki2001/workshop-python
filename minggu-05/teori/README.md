Ringkasan 

Input dan Ouput

Ada beberapa cara untuk mempresentasikan output dari suatu program; data dapat dicetak dalam bentuk 
yang dapat dibaca manusia, atau ditulis ke file untuk digunakan di masa mendatang. Bab ini akan 
membahas beberapa kemungkinan.
7.1. Pemformatan Keluaran Lebih Menarik
Sejauh ini kita menemukan dua cara penulisan nilai: pernyataan 
ekspresi dan print()fungsi. (Cara ketiga menggunakan write()metode objek file; file keluaran 
standar dapat dirujuk sebagai sys.stdout. Lihat Referensi Perpustakaan untuk informasi lebih 
lanjut tentang ini.)
Seringkali Anda menginginkan kontrol lebih besar atas pemformatan keluaran Anda daripada 
sekadar mencetak nilai yang dipisahkan oleh ruang. Ada beberapa cara untuk memformat 
output.
• Untuk menggunakan literal string terformat , awali string dengan fatau Fsebelum 
tanda kutip pembuka atau tanda kutip tiga. Di dalam string ini, Anda dapat menulis 
ekspresi Python antara karakter {dan }yang dapat merujuk ke variabel atau nilai 
literal.
• Metode str.format()string membutuhkan lebih banyak usaha manual. Anda masih akan 
menggunakan {dan }untuk menandai di mana variabel akan diganti dan dapat memberikan arahan 
pemformatan yang mendetail, tetapi Anda juga harus memberikan informasi yang akan diformat.
• Terakhir, Anda dapat melakukan semua penanganan string sendiri dengan menggunakan 
pemotongan string dan operasi penggabungan untuk membuat tata letak apa pun yang dapat Anda 
bayangkan. Tipe string memiliki beberapa metode yang melakukan operasi berguna untuk mengisi 
string ke lebar kolom tertentu.
Saat Anda tidak membutuhkan output mewah tetapi hanya ingin tampilan cepat dari beberapa variabel 
untuk keperluan debugging, Anda dapat mengonversi nilai apa pun menjadi string dengan 
fungsi repr()atau str().
Fungsi ini str()dimaksudkan untuk mengembalikan representasi nilai yang dapat dibaca oleh manusia, 
sementara repr()dimaksudkan untuk menghasilkan representasi yang dapat dibaca oleh penafsir (atau akan 
memaksa a SyntaxErrorjika tidak ada sintaks yang setara). Untuk objek yang tidak memiliki representasi 
khusus untuk konsumsi manusia, str()akan mengembalikan nilai yang sama dengan repr(). Banyak nilai, 
seperti angka atau struktur seperti daftar dan kamus, memiliki representasi yang sama menggunakan salah 
satu fungsi. String, khususnya, memiliki dua representasi berbeda.

