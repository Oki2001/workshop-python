#Ringkasan
Bab5.Struktur data
#Bab ini menjelaskan beberapa hal yang telah Anda pelajari secara lebih mendetail, dan menambahkan beberapa hal baru juga.
#Selengkapnya tentang Daftar 
Tipe data daftar memiliki beberapa metode lagi. Berikut ini semua metode objek daftar:
daftar. tambahkan ( x )
Tambahkan item ke akhir daftar. Setara dengan .a[len(a):] = [x]
daftar. memperpanjang ( dapat diubah )
Perpanjang daftar dengan menambahkan semua item dari iterable. Setara dengan .a[len(a):] = iterable
daftar. sisipkan ( i , x )
Masukkan item pada posisi tertentu. Argumen pertama adalah indeks elemen sebelum disisipkan, jadi sisipkan di bagian depan daftar, dan sama dengan .a.insert(0, x)a.insert(len(a), x)a.append(x)
Anda mungkin telah memperhatikan bahwa metode seperti insert, removeatau sortyang hanya mengubah daftar tidak memiliki nilai kembalian yang dicetak – mereka mengembalikan default None. 1 Ini adalah prinsip desain untuk semua struktur data yang bisa berubah di Python.
Hal lain yang mungkin Anda perhatikan adalah tidak semua data dapat diurutkan atau dibandingkan. Misalnya, tidak mengurutkan karena bilangan bulat tidak dapat dibandingkan dengan string dan Tidak ada yang tidak dapat dibandingkan dengan tipe lainnya. Selain itu, ada beberapa tipe yang tidak memiliki relasi pengurutan yang ditentukan. Misalnya, bukan perbandingan yang valid.[None, 'hello', 10]3+4j < 5+7j
#Menggunakan Daftar sebagai Tumpukan 
Metode daftar membuatnya sangat mudah untuk menggunakan daftar sebagai tumpukan, di mana elemen terakhir yang ditambahkan adalah elemen pertama yang diambil (“last-in, first-out”). Untuk menambahkan item ke atas tumpukan, gunakan append(). Untuk mengambil item dari atas tumpukan, gunakan pop()tanpa indeks eksplisit
#Menggunakan Daftar sebagai Antrean ¶
Dimungkinkan juga untuk menggunakan daftar sebagai antrian, di mana elemen pertama yang ditambahkan adalah elemen pertama yang diambil (“first-in, first-out”); namun, daftar tidak efisien untuk tujuan ini. Sementara menambahkan dan muncul dari akhir daftar cepat, melakukan sisipan atau muncul dari awal daftar lambat (karena semua elemen lain harus digeser satu).
#Daftar Pemahaman 
Pemahaman daftar menyediakan cara ringkas untuk membuat daftar. Aplikasi umum adalah membuat daftar baru di mana setiap elemen adalah hasil dari beberapa operasi yang diterapkan ke setiap anggota urutan lain atau iterable, atau untuk membuat urutan elemen yang memenuhi kondisi tertentu.
