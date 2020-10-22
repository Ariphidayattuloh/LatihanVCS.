#Latihan-VCS

# Latihan-VCS
#  LatihanVCS Membuat satu repositori LatihanVCS dan Buat file README.md

Nama: Arip Hidayattuloh

Nim: 312010244

Kelas: TI.20.B.1

Pemilihan: Agung Nugroho S.Kom, M.kom


Instalasi Git

• Download Git, buka website resminya Git (git-scm.com).

![1](https://user-images.githubusercontent.com/72840534/96370052-cd255d80-1186-11eb-9b0f-7d376a4b2499.png)


• Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau menggunakan 64bit, unduh yang 64bit. Begitu juga kalau menggunakan 32bit.


!(https://user-images.githubusercontent.com/72840534/96367580-f63ef180-1178-11eb-96b6-5dda04c64fdd.jpg)


! [ gambar 3 ] (https://user-images.githubusercontent.com/72840534/96367595-08209480-1179-11eb-9fdb-cf8707a157de.jpg)


Selamat, Git sudah terinstal di Windows. Untuk tiba-tiba, silahkan buka CMD atau PowerShell, kemudian ketik perintah

git --version

! [ gambar 4 ] (https://user-images.githubusercontent.com/72840534/96367601-0d7ddf00-1179-11eb-8dd6-ef2dee401a8c.jpg)

Menyusun Konfigurasi Global

• Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

• tata bahasa ini bisa dilakukan untuk penyimpanan global atau penyimpanan individu.

• sebelum dilakukan konfigurasi, terjadi kegagalan saat menjalankan perintah git commit

• Konfigurasi Repositori Global

$ git config --pengguna global. nama “nama_user”

$ git config --pengguna global. email “nama_user”

! [ gambar 5 1 ] (https://user-images.githubusercontent.com/72840534/96367605-1373c000-1179-11eb-9e18-bb2f1afc882b.jpg)


Membuat Reposiory Lokal

• Buka direktory aktif, misal: c: \ l abs_pemrograman1 (buka menggunakan Windows Explorer)

• klik kanan pada direktori aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

• Buat praktikum proyek direktory pertama dengan nama Latihan-VCS

$ mkdir Latihan-VCS

$ cd Latihan-VCS

! [ gambar 6 ] (https://user-images.githubusercontent.com/72840534/96367610-1b336480-1179-11eb-9d37-7be4625bdcad.jpg)

• Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (ubah direktori)

• direktori aktif menjadi: c: \ l abs_pemrograman1 \ L atihan-VCS

Membuat Reposiory Lokal

• Jalankan perintah git init, untuk membuat repositori lokal.

$ git init

! [ gambar 7 ] (https://user-images.githubusercontent.com/72840534/96367612-1e2e5500-1179-11eb-89f5-fd2f94acffea.jpg)


• Repositori baru berhasil inisialisasi, dengan terbentuknya satu Direktori yang tersembunyi dengan nama .git

! [ gambar 8 ] (https://user-images.githubusercontent.com/72840534/96367614-21294580-1179-11eb-97a4-516a82407145.jpg)

• Pada direktori tersebut, semua perubahan pada direktori kerja akan disimpan.

Menambahkan file baru pada repositori

• Untuk membuat file dapat menggunakan editor teks, lalu menyimpan filenya pada direktori aktif (repository)

• disini kita akan coba buat satu file bernama README.md (text file)

$ echo “# Latihan-VCS” >> README. md

! [ echo1 ] (https://user-images.githubusercontent.com/72840534/96368045-af9ec680-117b-11eb-81b6-6b4a8f7e4f1d.png)

• File README.md berhasil dibuat.

! [ readme ] (https://user-images.githubusercontent.com/72840534/96368179-b11cbe80-117c-11eb-8ba4-2de88299c570.jpg)

Menambahkan file baru pada repositori

• Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

$ git tambahkan README. md

• File README.md berhasil ditambahkan

! [ readm berhasil ] (https://user-images.githubusercontent.com/72840534/96368438-060d0480-117e-11eb-97d7-59da7d7d23bb.jpg)


Commit (Menyimpan perubahan ke database)

• Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”

$ git commit -m “Bahasa Pemrograman Repository Lokal LatihanVCS"

! [ baca COMMIT ] (https://user-images.githubusercontent.com/72840534/96368607-d27eaa00-117e-11eb-973b-1148d683b9be.jpg)


• Perubahan berhasil disimpan

! [ BUKA FILE ] (https://user-images.githubusercontent.com/72840534/96368701-88e28f00-117f-11eb-811f-e05fa64d404b.jpg)

Membuat server repositori

• Server reopsitory yang akan kita gunakan adalah http://github.com

• Anda harus membuat akun terlebih dahulu.

• Pada laman github, klik tombol start a project, atau

• Dari menu (icon +) klik New Repository

! [ repositori baru ] (https://user-images.githubusercontent.com/72840534/96368967-386c3100-1181-11eb-9766-aaddc753338d.jpg)

Membuat server repositori

• Isi nama repositorynya, misal: LatihanVCS.

! [ membuat repository ] (https://user-images.githubusercontent.com/72840534/96369183-b7159e00-1182-11eb-86f5-2074e6750b05.png)
• lalu klik tombol Buat repositori


Setel Remote Repository

• Remote Repository merupakan repository server yang akan

digunakan untuk menyimpan setiap perubahan pada repositori lokal, sehingga dapat diakses oleh banyak pengguna.

Alamat url kita

! [ REMOTE ] (https://user-images.githubusercontent.com/72840534/96369409-e547ad80-1183-11eb-9224-5633948b042a.png)

• Untuk menambahkan server repositori jarak jauh, gunakan perintah git remote add origin [url]

$ git jarak jauh tambahkan asal https://github.com/ariphidayattuloh/LatihanVCS.git

! [ tambahkan ] (https://user-images.githubusercontent.com/72840534/96369473-5d15d800-1184-11eb-9627-0430787fe721.png)



Push (mengirim perubahan ke server)

• Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

$ git push -u master asal

• Perintah ini akan memasukkan username dan password pada akun github.com

! [ masuk ] (https://user-images.githubusercontent.com/72840534/96369637-694e6500-1185-11eb-941a-2a4f4e7988e6.png)


! [ asal ] (https://user-images.githubusercontent.com/72840534/96369703-c813de80-1185-11eb-9f77-f605975e2a27.png)



Melihat hasil pada repositori server

• Buka laman github.com, khusus pada repositorinya.

• Maka perubahan akan terlihat pada laman tersebut.



! [ 222 ] (https://user-images.githubusercontent.com/72840534/96371614-af5af700-118c-11eb-939c-5e8fba1ad2ec.png)

Gandakan Repositori

• Clone repository, pada kenyataan adalah meng-copy server repositori dan secara otomatis membuat satu direktori sesuai dengan nama repositorynya (direktori kerja).

• Untuk melakukan cloning, gunakan perintah git clone [url]

$ git clone https://github.com/ariphidayattuloh/LatihanVCS.git


! [ asal ] (https://user-images.githubusercontent.com/72840534/96369703-c813de80-1185-11eb-9f77-f605975e2a27.png)




File Kegunaan README.md

• Apabila kita menggunakan github, untuk memberikan penjelasan awal pada proyek yang kita, maka dapat menggunakan sebuah file yang bernama README.md

• Pada file tersebut kita dapat membuat dokumentasi awal dari setiap proyek yang kita buat untuk memberikan penjelasan atau hanya menggunakan cara penggunaan dari aplikasi yang kita kembangkan.

• Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan format Markdown.

• untuk lebih jelasnya, dapat anda gunakan cara penggunaan markdown


! [ 6efb9bc5d143-article-190612-github-body-text ] (https://user-images.githubusercontent.com/72840534/96370606-9d775500-1188-11eb-88dc-43e57f206245.jpg)
