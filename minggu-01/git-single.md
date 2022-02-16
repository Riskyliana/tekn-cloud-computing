**SCM: Git dan GitHub**

**Instalasi Git (Versi 2.35.1.2)**
1. Setelah download Git, double click pada file yang telah berhasil di-download. Akan muncul lisensi. Klik Next untuk lanjut.

1. Setelah itu, pilih lokasi instalasi. Secara default akan terisi C:\Program Files\Git. Ganti lokasi jika memang menginginkan lokasi lain. Klik Next untuk lanjut.

1. Pilih komponen. Tidak perlu diubah-ubah, sesuai dengan default saja. Klik Next untuk lanjut.

1. Mengisi shortcut untuk menu Start. Gunakan default (Git), ganti jika ingin mengganti - misalnya Git VCS.

1. Pilih editor yang akan digunakan bersama dengan Git. Pada pilihan ini, menggunakan Vim Editor.

1. Menyesuaikan nama branch awal di repositori baru.

1. Selanjutnya adalah pengaturan Path Environment. Path Environment berfungsi untuk mengeksekusi perintah perintah pada Git. Pilih Git from the command line and also from 3rd-party software agar saat menjalankan perintah Git dapat dikenali di Command Prompt (CMD) pada Windows

1. Kemudian untuk mengeksekusi SSH, Anda bisa menggunakan aplikasi dari Git atau  dari platform lain seperti PuTTY dan Bitvise. Pada tutorial ini kami menggunakan Use OpenSSH, aplikasi default SSH dari Git. Klik Next untuk melanjutkan instalasi.

1. Pilih OpenSSL untuk HTTPS. Git menggunakan https untuk akes ke repo GitHub atau repo-repo lain (GitLab, Assembla).


1. Pilih pilihan pertama untuk konversi akhir baris (CR-LF).

1. Pilih PuTTY untuk terminal yang digunakan untuk mengakses Git Bash.

1. Pilih default dari “git pull”.

1. Pilih credensial helper

1. Untuk opsi ekstra, pilih serta aktifkan 1

1. Setelah menambahkan konfigurasi ekstra pada Git, Anda bisa memulai proses instalasi Git. Klik Install untuk melanjutkan proses.

1. Setelah itu proses instalasi akan dilakukan.

1. Jika selesai akan muncul dialog pemberitahuan. Klik pada Finish.

1. Untuk menjalankan, dari Start menu, ketikkan "Git", akan muncul beberapa pilihan. Pilih "Git Bash" atau "Git GUI".

1. Tampilan jika akan menggunakan "Git Bash"

1. Tampilan jika akan menggunakan "Git GUI"

1. Untuk mencoba dari command prompt, masuk ke command prompt, setelah itu eksekusi "git --version" untuk melihat apakah sudah terinstall atau belum. Jika sudah terinstall dengan benar, makan akan muncul hasil berikut:


1. **Konfigurasi Git**
1. Mengelola Repo Sendiri

$ git config --global user.name "Nama Anda di GitHub"

$ git config --global user.email <email@domain.tld>

$ git config --list



1. **Mengelola Repo Sendiri**
- Mengelola repo di account sendiri

**Membuat Repo**

1. Klik tanda + pada bagian atas setelah login, pilih New repository

1. Isikan nama, keterangan, serta lisensi. Jika dikehendaki, bisa membuat repo Private

1. Klik Create Repository

**Clone Repo**

Proses clone adalah proses untuk menduplikasikan remote repo di GitHub ke komputer lokal. Untuk melakukan proses clone, gunakan perintah berikut:

Setelah perintah ini, di direktori awesome-project akan disimpan isi repo yang sama dengan di GitHub. Perbedaannya, di komputer lokal terdapat direktori .git yang digunakan secara internal oleh Git.

**Mengelola Repo**

Mengubah Isi - Push Tanpa Branching dan Merging


Cara ini lebih mudah tetapi mempunyai resiko jika terjadi kesalahan dalam edit. Cara yang lebih aman tetapi memerlukan langkah yang lebih panjang adalah branching and merging

Mengubah Isi dengan Branching and Merging

Dengan menggunakan cara ini, setiap kali akan melakukan perubaham, perubahan itu dilakukan di komputer lokal dengan membuat suatu cabang yang nantinya digunakan untuk menampung perubahan-perubahan tersebut. Setelah itu, cabang itu yang akan dikirim ke repo GitHub untuk dimintai review kemudian digabungkan (merge) ke master. Secara umum, repo yang dibuat biasanya sudah mempunyai satu branch yang disebut dengan master. Cara ini lebih aman, terstruktur, terkendali, dan mempunyai history yang lebih baik. Jika perubahan yang kita buat sudah terlalu kacau dan kita menyesal, maka ada cara untuk "membersihkan" repo lokal kita. Secara umum, langkahnya adalah sebagai berikut:

1) Buat branch untuk menampung perubahan-perubahan

1) Lakukan perubahan-perubahan

1) Add dan commit perubahan-perubahan tersebut ke branch

1) Kembali ke repo main dan melakukan push

1) Buat pull request di GitHub

1) Merge pull request di GitHub

1) Setelah itu, Confirm Merge, untuk menampung perubahan-perubahan tersebut ke master.

1) Setelah itu, merge di komputer lokal:


Sinkronisasi

Suatu saat, bisa saja terjadi kita menggunakan komputer lain dan mengedit repo melalui repo lokal di komputer lain, setelah itu pindah ke kamputer lain lagi. Saat itu, kita perlu melakukan sinkronisasi ke kemputer lokal. Perintah untuk sinkronisasi adalah:

$ git pull

Membatalkan Perubahan


Undo Commit Terakhir

Suatu saat, mungkin kita sudah terlanjur mem-push perubahan ke repo GitHub, setelah itu kita baru menyadari bahwa perubahan tersebut salah. Untuk itu, kita bisa melakukan git revert.



Contoh di atas adalah contoh untuk mengubah README.md dengan beberapa commit. Setelalh itu, kita akan mengembalikan ke posisi terakhir sebelum commit terakhir.

Selanjutnya, tinggal di-push ke repo GitHub.

Jika commit sudah dilakukan, tetapi belum di-push ke repo GitHub (masih berada di lokal), cara membatalkannya:

Untuk kembali ke perubahan pada saat yang sudah lama, yang perlu dilakukan adalah melakukan git revert <posisi> kemudian mengedit secara manual kemudian push ke repo.

- Mengelola repo di organisasi

Repo yang dibuat bisa diletakkan pada account kita maupun berada pada suatu organisasi. Organisasi bisa kita buat sendiri maupun kita dimasukkan menjadi anggota organisasi. Pada dasarnya, bagian ini sama dengan bagian sebelumnya, hanya saja, pada saat membuat repo Owner dari repo adalah organisasi.

**TUGAS**

**Kolaborasi**

**Fork**

Fork adalah membuat clone dari suatu repo di GitHub milik upstream author, diletakkan ke milik kontributor. Fork hanya dilakukan sekali saja. Pada dasarnya, proses untuk fork ini meliputi:

1) Fork repo di web GitHub.
1) Clone fork tersebut di komputer lokal.

Kontributor harus mem-fork repo upstream author sehingga di repo kontributor muncul repo tersebut. Proses forking ini dijelaskan dengan langkah-langkah berikut:

1) Login ke GitHub
1) Akses repo yang akan di-fork: https://github.com/novirachmahwati/playground
1) Pada sisi kanan atas, klik Fork:

1) Setelah proses, repo dari upstream author sudah berada di account GitHub kita (kontributor)

Setelah proses tersebut, clone di komputer lokal:

Setelah itu, konfigurasikan repo lokal kontributor. Pada kondisi saat ini, di komputer lokal sudah terdapat repo playground-1 yang berada pada direktori dengan nama yang sama. Untuk keperluan berkontribusi, ada 2 nama repo yang harus diatur:

1) origin: menunjuk ke repo milik kontributor di GitHub, hasil dari fork.
1) upstream: menunjuk ke repo milik upstream author (repo asli) di account oldstager.

Repo origin sudah dituliskan konfigurasinya pada saat melakukan proses clone dari repo kontributor. Konfigurasi repo upstream harus dibuat.

Tambahkan remote upstream:

Hasil


**Mengirimkan Pull Request**

Setiap kali melakukan perubahan, kirim perubahan tersebut. Pengiriman ini disebut dengan Pull Request. Pada posisi ini, kontributor bisa mengirimkan kontribusi dengan cara mengirimkan pull request (PR) ke upstream author. Secara umum, langkah-langkahnya adalah sebagai berikut:

1) Kontributor akan bekerja di repo lokal (create, update, delete isi)
1) Commit
1) Push ke repo kontributor
1) Kirimkan PR ke repo upstream author.
1) Upstream author me-review dan kemudian menyetujui (merge) ke master atau menolak PR.
1) Jika disetujui dan di-merge ke repo master dari upstream author, sinkronkan repo di komputer lokal dan repo GitHub kontributor.

**Membuat Perubahan di Repo Lokal**

Sebelum melakukan perubahan, pastikan:

1) Sudah ada koordinasi secara manual tentang perubahan-perubahan yang akan dilakukan.
1) Setelah melakukan perubahan-perubahan, pastikan bahwa isi repo lokal tersinkronisasi dengan repo dari upstream author.
1) Cara melakukan sinkronisasi:

1) Lakukan perubahan-perubahan, setelah itu push ke origin (milik kontributor)

1) Setelah itu, buka halaman Web dari repo kontributor https://github.com/Riskyliana/playground. Pada halaman tersebut akan ditampilkan isi yang kita push.

1) Pilih Compare and pull request, kemudian isikan deskripsi PR dan klik pada Create pull request:

1) Pada repo upstream author, muncul angka 1 (artinya jumlahnya 1) pada Pull requests di bagian atas.
1) Upstream author bisa menyetujui setelah melakukan review: klik pada Pull requests, akan muncul PR dengan message seperti yang ditulis oleh kontributor (Add: contributor). Klik pada PR tersebut, review kemudian klik Merge pull request diikuti dengan Confirm merge. Setelah itu, status akan berubah menjadi Merged.
1) Sinkronkan semua repo (lokal maupun GitHub kontributor)



**Konflik**

Ada kemungkinan, jika satu orang mengirimkan PR untuk satu atau lebih file dan sementara itu ada lainnya juga yang mengirimkan PR pada satu atau lebih file yang sama, maka akan terjadi konflik karena ada satu atau lebih file yang sama yang di-edit dan akan di-merge. Jika sampai terjadi kasus seperti ini, maka upatream author harus menolak semua PR dan kemudian masing-masing kontributor diharapkan menyelesaikan secara manual (offline) kemudian memutuskan siapa yang akan mengirimkan PR.




