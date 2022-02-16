<h1>Instalasi Git (Versi 2.35.1.2)</h1>

1. Setelah download Git, double click pada file yang telah berhasil di-download. Akan muncul lisensi. Klik Next untuk lanjut.
![image](https://user-images.githubusercontent.com/41459086/154255588-d59c4120-366e-414f-84a8-762fe7aba127.png)

1. Setelah itu, pilih lokasi instalasi. Secara default akan terisi C:\Program Files\Git. Ganti lokasi jika memang menginginkan lokasi lain. Klik Next untuk lanjut.
![image](https://user-images.githubusercontent.com/41459086/154255597-7204983a-6559-43b1-bcb9-4042bef99dd3.png)

1. Pilih komponen. Tidak perlu diubah-ubah, sesuai dengan default saja. Klik Next untuk lanjut.
![image](https://user-images.githubusercontent.com/41459086/154255610-34aac3b9-dc86-4c0b-9fa3-13ba741915b1.png)

1. Mengisi shortcut untuk menu Start. Gunakan default (Git), ganti jika ingin mengganti - misalnya Git VCS.
![image](https://user-images.githubusercontent.com/41459086/154255617-186249ab-4789-4cd1-bde6-de04d51c055e.png)

1. Pilih editor yang akan digunakan bersama dengan Git. Pada pilihan ini, menggunakan Vim Editor.
![image](https://user-images.githubusercontent.com/41459086/154255639-daefa93d-d47a-4d84-90a8-a22b9c9002e9.png)

1. Menyesuaikan nama branch awal di repositori baru.
![image](https://user-images.githubusercontent.com/41459086/154255659-aefe30b6-3ea8-40d4-9025-088f5d96b13a.png)

1. Selanjutnya adalah pengaturan Path Environment. Path Environment berfungsi untuk mengeksekusi perintah perintah pada Git. Pilih Git from the command line and also from 3rd-party software agar saat menjalankan perintah Git dapat dikenali di Command Prompt (CMD) pada Windows
![image](https://user-images.githubusercontent.com/41459086/154255675-62e916cb-ce77-4bff-b7b4-9c00c7c38d57.png)

1. Kemudian untuk mengeksekusi SSH, Anda bisa menggunakan aplikasi dari Git atau  dari platform lain seperti PuTTY dan Bitvise. Pada tutorial ini kami menggunakan Use OpenSSH, aplikasi default SSH dari Git. Klik Next untuk melanjutkan instalasi.
![image](https://user-images.githubusercontent.com/41459086/154255691-09057838-e402-42d3-816d-4f4a1b73f08e.png)

1. Pilih OpenSSL untuk HTTPS. Git menggunakan https untuk akes ke repo GitHub atau repo-repo lain (GitLab, Assembla).
![image](https://user-images.githubusercontent.com/41459086/154255713-82c6522f-c80e-49cd-8d37-934e84cccf76.png)

1. Pilih pilihan pertama untuk konversi akhir baris (CR-LF).
![image](https://user-images.githubusercontent.com/41459086/154255734-bcb39299-35b2-48a0-be91-440e4e3bf517.png)

1. Pilih PuTTY untuk terminal yang digunakan untuk mengakses Git Bash.
![image](https://user-images.githubusercontent.com/41459086/154255757-bd7acabf-e905-4a95-8362-3e5cc8936cb3.png)

1. Pilih default dari “git pull”.
![image](https://user-images.githubusercontent.com/41459086/154255769-351c3042-239d-4cdd-a5f7-7bdffdbf94e8.png)

1. Pilih credensial helper
![image](https://user-images.githubusercontent.com/41459086/154255783-ff0b0ffc-2aa5-43a6-9357-0ba7df37e35d.png)

1. Untuk opsi ekstra, pilih serta aktifkan 1
![image](https://user-images.githubusercontent.com/41459086/154255798-85991ad7-fb09-4661-ba89-9c600a332c4d.png)

1. Setelah menambahkan konfigurasi ekstra pada Git, Anda bisa memulai proses instalasi Git. Klik Install untuk melanjutkan proses.
![image](https://user-images.githubusercontent.com/41459086/154255812-5c04b57f-a864-49a3-9ff4-2ae146523866.png)

1. Setelah itu proses instalasi akan dilakukan.
![image](https://user-images.githubusercontent.com/41459086/154255828-04740508-21e6-4ae0-a4a0-4fde752d8fe8.png)

1. Jika selesai akan muncul dialog pemberitahuan. Klik pada Finish.
![image](https://user-images.githubusercontent.com/41459086/154255843-24040d89-8c4e-4ac4-882d-51acc71228cc.png)

1. Untuk menjalankan, dari Start menu, ketikkan "Git", akan muncul beberapa pilihan. Pilih "Git Bash" atau "Git GUI".
![image](https://user-images.githubusercontent.com/41459086/154255867-9628f899-be23-4455-ac6d-891b7c9d5468.png)

1. Tampilan jika akan menggunakan "Git Bash"
![image](https://user-images.githubusercontent.com/41459086/154255892-57ed56a2-f02b-4421-b014-c3cabe8380df.png)

1. Tampilan jika akan menggunakan "Git GUI"
![image](https://user-images.githubusercontent.com/41459086/154255899-07ad23a2-b8f6-41c7-8a57-9d05dda182cf.png)

1. Untuk mencoba dari command prompt, masuk ke command prompt, setelah itu eksekusi "git --version" untuk melihat apakah sudah terinstall atau belum. Jika sudah terinstall dengan benar, makan akan muncul hasil berikut:
![image](https://user-images.githubusercontent.com/41459086/154255916-71ba4907-94cf-4866-8b39-18ba8e839cd8.png)


<h1>Konfigurasi Git</h1>

$ git config --global user.name "Nama Anda di GitHub"

$ git config --global user.email <email@domain.tld>

$ git config --list

![image](https://user-images.githubusercontent.com/41459086/154255944-12f4ad29-180d-48ea-a21d-32ee9c0605ec.png)

  
<h1>Mengelola Repo Sendiri</h1>
<h2>Mengelola repo di account sendiri</h2>

<h3>Membuat Repo</h3>

1. Klik tanda + pada bagian atas setelah login, pilih New repository
![image](https://user-images.githubusercontent.com/41459086/154255967-b3bf1966-3df0-4dcd-9853-da5c6e398386.png)

1. Isikan nama, keterangan, serta lisensi. Jika dikehendaki, bisa membuat repo Private
![image](https://user-images.githubusercontent.com/41459086/154255976-c9c5fd45-3672-43f2-8175-acbabe487e10.png)

1. Klik Create Repository

<h3>Clone Repo</h3>

Proses clone adalah proses untuk menduplikasikan remote repo di GitHub ke komputer lokal. Untuk melakukan proses clone, gunakan perintah berikut:
![image](https://user-images.githubusercontent.com/41459086/154256003-47424d5b-5e6b-4ba4-96d6-6b6cd4f8427b.png)

Setelah perintah ini, di direktori awesome-project akan disimpan isi repo yang sama dengan di GitHub. Perbedaannya, di komputer lokal terdapat direktori .git yang digunakan secara internal oleh Git.

<h3>Mengelola Repo</h3>

**Mengubah Isi - Push Tanpa Branching dan Merging**
![image](https://user-images.githubusercontent.com/41459086/154256033-a8d09f4d-65bf-4bd6-a0f0-39f753f25ffd.png)
![image](https://user-images.githubusercontent.com/41459086/154256053-16b997c6-2e9d-4231-a3a2-7a9d1b8b758b.png)

Cara ini lebih mudah tetapi mempunyai resiko jika terjadi kesalahan dalam edit. Cara yang lebih aman tetapi memerlukan langkah yang lebih panjang adalah branching and merging

**Mengubah Isi dengan Branching and Merging**

Dengan menggunakan cara ini, setiap kali akan melakukan perubaham, perubahan itu dilakukan di komputer lokal dengan membuat suatu cabang yang nantinya digunakan untuk menampung perubahan-perubahan tersebut. Setelah itu, cabang itu yang akan dikirim ke repo GitHub untuk dimintai review kemudian digabungkan (merge) ke master. Secara umum, repo yang dibuat biasanya sudah mempunyai satu branch yang disebut dengan master. Cara ini lebih aman, terstruktur, terkendali, dan mempunyai history yang lebih baik. Jika perubahan yang kita buat sudah terlalu kacau dan kita menyesal, maka ada cara untuk "membersihkan" repo lokal kita. Secara umum, langkahnya adalah sebagai berikut:

1) Buat branch untuk menampung perubahan-perubahan
![image](https://user-images.githubusercontent.com/41459086/154256080-f15aac66-01e2-4789-b043-a63b28bcbdd2.png)

1) Lakukan perubahan-perubahan
![image](https://user-images.githubusercontent.com/41459086/154256092-dc0e00a2-b3af-4856-8d7b-364fae26e7ee.png)

1) Add dan commit perubahan-perubahan tersebut ke branch
![image](https://user-images.githubusercontent.com/41459086/154256102-72e406bd-6eee-426f-9837-b50dc0326548.png)

1) Kembali ke repo main dan melakukan push
![image](https://user-images.githubusercontent.com/41459086/154256113-02ef308d-19d9-474c-bcd7-a1fed82c20f5.png)

1) Buat pull request di GitHub
![image](https://user-images.githubusercontent.com/41459086/154256128-edb3f9eb-4688-4e7d-a8fe-aa5278a916fe.png)

1) Merge pull request di GitHub
![image](https://user-images.githubusercontent.com/41459086/154256138-174c1b1f-7485-4c8d-9df5-5ddeb1fb51a9.png)

1) Setelah itu, Confirm Merge, untuk menampung perubahan-perubahan tersebut ke master.
![image](https://user-images.githubusercontent.com/41459086/154256160-0c975332-a11f-4727-9a06-2457c9674e13.png)

1) Setelah itu, merge di komputer lokal:
![image](https://user-images.githubusercontent.com/41459086/154256171-351d8057-627c-4aec-a74a-42f9c7e91c1b.png)


**Sinkronisasi**

Suatu saat, bisa saja terjadi kita menggunakan komputer lain dan mengedit repo melalui repo lokal di komputer lain, setelah itu pindah ke kamputer lain lagi. Saat itu, kita perlu melakukan sinkronisasi ke kemputer lokal. Perintah untuk sinkronisasi adalah:

```bash
$ git pull
```

**Membatalkan Perubahan**

![image](https://user-images.githubusercontent.com/41459086/154256194-71234bb1-263d-4e6c-8a54-748a5cc3f8f5.png)
![image](https://user-images.githubusercontent.com/41459086/154256211-f12dd79b-9363-4594-8e71-44c3b038d274.png)

**Undo Commit Terakhir**

Suatu saat, mungkin kita sudah terlanjur mem-push perubahan ke repo GitHub, setelah itu kita baru menyadari bahwa perubahan tersebut salah. Untuk itu, kita bisa melakukan git revert.
![image](https://user-images.githubusercontent.com/41459086/154256258-1bc8ab80-1de2-48e2-bc69-a87ecd3bd955.png)
![image](https://user-images.githubusercontent.com/41459086/154256319-5754102a-4fb4-43be-9774-cc1e99bcf0d6.png)
![image](https://user-images.githubusercontent.com/41459086/154256342-e42a1527-7068-483d-94cb-5dc194e05b98.png)
![image](https://user-images.githubusercontent.com/41459086/154256368-f68bb950-2c46-4801-8079-c0504b29f042.png)

Contoh di atas adalah contoh untuk mengubah README.md dengan beberapa commit. Setelalh itu, kita akan mengembalikan ke posisi terakhir sebelum commit terakhir.
![image](https://user-images.githubusercontent.com/41459086/154256388-7b45ccbe-9a38-40d4-aa10-9808e1fe3b7b.png)

Selanjutnya, tinggal di-push ke repo GitHub.
![image](https://user-images.githubusercontent.com/41459086/154256400-260e0597-d673-42c2-8c90-dc682c27e45f.png)
![image](https://user-images.githubusercontent.com/41459086/154256420-35790430-32eb-410a-8b28-e2b197e1796a.png)

Jika commit sudah dilakukan, tetapi belum di-push ke repo GitHub (masih berada di lokal), cara membatalkannya:
![image](https://user-images.githubusercontent.com/41459086/154256433-300d8c71-c38f-4669-9cd6-18785215374e.png)
![image](https://user-images.githubusercontent.com/41459086/154256442-cf1f862b-8cf6-4d73-b2b3-1e95d0aaee74.png)

Untuk kembali ke perubahan pada saat yang sudah lama, yang perlu dilakukan adalah melakukan git revert <posisi> kemudian mengedit secara manual kemudian push ke repo.

 <h3>Mengelola repo di organisasi</h3>

Repo yang dibuat bisa diletakkan pada account kita maupun berada pada suatu organisasi. Organisasi bisa kita buat sendiri maupun kita dimasukkan menjadi anggota organisasi. Pada dasarnya, bagian ini sama dengan bagian sebelumnya, hanya saja, pada saat membuat repo Owner dari repo adalah organisasi.

