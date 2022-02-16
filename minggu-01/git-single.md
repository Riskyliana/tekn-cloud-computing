<h1>Instalasi Git (Versi 2.35.1.2)</h1>

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


<h1>Konfigurasi Git</h1>

$ git config --global user.name "Nama Anda di GitHub"

$ git config --global user.email <email@domain.tld>

$ git config --list

  
<h1>Mengelola Repo Sendiri</h1>
<h2>Mengelola repo di account sendiri</h2>

<h3>Membuat Repo</h3>

1. Klik tanda + pada bagian atas setelah login, pilih New repository

1. Isikan nama, keterangan, serta lisensi. Jika dikehendaki, bisa membuat repo Private

1. Klik Create Repository

<h3>Clone Repo</h3>

Proses clone adalah proses untuk menduplikasikan remote repo di GitHub ke komputer lokal. Untuk melakukan proses clone, gunakan perintah berikut:

Setelah perintah ini, di direktori awesome-project akan disimpan isi repo yang sama dengan di GitHub. Perbedaannya, di komputer lokal terdapat direktori .git yang digunakan secara internal oleh Git.

<h3>Mengelola Repo</h3>

**Mengubah Isi - Push Tanpa Branching dan Merging**


Cara ini lebih mudah tetapi mempunyai resiko jika terjadi kesalahan dalam edit. Cara yang lebih aman tetapi memerlukan langkah yang lebih panjang adalah branching and merging

**Mengubah Isi dengan Branching and Merging**

Dengan menggunakan cara ini, setiap kali akan melakukan perubaham, perubahan itu dilakukan di komputer lokal dengan membuat suatu cabang yang nantinya digunakan untuk menampung perubahan-perubahan tersebut. Setelah itu, cabang itu yang akan dikirim ke repo GitHub untuk dimintai review kemudian digabungkan (merge) ke master. Secara umum, repo yang dibuat biasanya sudah mempunyai satu branch yang disebut dengan master. Cara ini lebih aman, terstruktur, terkendali, dan mempunyai history yang lebih baik. Jika perubahan yang kita buat sudah terlalu kacau dan kita menyesal, maka ada cara untuk "membersihkan" repo lokal kita. Secara umum, langkahnya adalah sebagai berikut:

1) Buat branch untuk menampung perubahan-perubahan

1) Lakukan perubahan-perubahan

1) Add dan commit perubahan-perubahan tersebut ke branch

1) Kembali ke repo main dan melakukan push

1) Buat pull request di GitHub

1) Merge pull request di GitHub

1) Setelah itu, Confirm Merge, untuk menampung perubahan-perubahan tersebut ke master.

1) Setelah itu, merge di komputer lokal:


**Sinkronisasi**

Suatu saat, bisa saja terjadi kita menggunakan komputer lain dan mengedit repo melalui repo lokal di komputer lain, setelah itu pindah ke kamputer lain lagi. Saat itu, kita perlu melakukan sinkronisasi ke kemputer lokal. Perintah untuk sinkronisasi adalah:

```bash
$ git pull
```

Membatalkan Perubahan


**Undo Commit Terakhir**

Suatu saat, mungkin kita sudah terlanjur mem-push perubahan ke repo GitHub, setelah itu kita baru menyadari bahwa perubahan tersebut salah. Untuk itu, kita bisa melakukan git revert.



Contoh di atas adalah contoh untuk mengubah README.md dengan beberapa commit. Setelalh itu, kita akan mengembalikan ke posisi terakhir sebelum commit terakhir.

Selanjutnya, tinggal di-push ke repo GitHub.

Jika commit sudah dilakukan, tetapi belum di-push ke repo GitHub (masih berada di lokal), cara membatalkannya:

Untuk kembali ke perubahan pada saat yang sudah lama, yang perlu dilakukan adalah melakukan git revert <posisi> kemudian mengedit secara manual kemudian push ke repo.

 <h3>Mengelola repo di organisasi</h3>

Repo yang dibuat bisa diletakkan pada account kita maupun berada pada suatu organisasi. Organisasi bisa kita buat sendiri maupun kita dimasukkan menjadi anggota organisasi. Pada dasarnya, bagian ini sama dengan bagian sebelumnya, hanya saja, pada saat membuat repo Owner dari repo adalah organisasi.

