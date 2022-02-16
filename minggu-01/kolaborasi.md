<h1>Kolaborasi</h1>

<h3>Fork</h3>

Fork adalah membuat clone dari suatu repo di GitHub milik upstream author, diletakkan ke milik kontributor. Fork hanya dilakukan sekali saja. Pada dasarnya, proses untuk fork ini meliputi:

1) Fork repo di web GitHub.
1) Clone fork tersebut di komputer lokal.

Kontributor harus mem-fork repo upstream author sehingga di repo kontributor muncul repo tersebut. Proses forking ini dijelaskan dengan langkah-langkah berikut:

1) Login ke GitHub
1) Akses repo yang akan di-fork: https://github.com/novirachmahwati/playground
1) Pada sisi kanan atas, klik Fork:
![image](https://user-images.githubusercontent.com/41459086/154254635-81718dff-6526-4d7d-8b6c-2a4145aa35e9.png)

1) Setelah proses, repo dari upstream author sudah berada di account GitHub kita (kontributor)
![image](https://user-images.githubusercontent.com/41459086/154254621-b306f703-ad9f-4bf0-8c5b-d70f7d0e7d11.png)

Setelah proses tersebut, clone di komputer lokal:
![image](https://user-images.githubusercontent.com/41459086/154254601-f292bac9-b8c0-4ce5-884b-4174f91c7699.png)

Setelah itu, konfigurasikan repo lokal kontributor. Pada kondisi saat ini, di komputer lokal sudah terdapat repo playground-1 yang berada pada direktori dengan nama yang sama. Untuk keperluan berkontribusi, ada 2 nama repo yang harus diatur:

1) origin: menunjuk ke repo milik kontributor di GitHub, hasil dari fork.
1) upstream: menunjuk ke repo milik upstream author (repo asli) di account oldstager.

Repo origin sudah dituliskan konfigurasinya pada saat melakukan proses clone dari repo kontributor. Konfigurasi repo upstream harus dibuat.
![image](https://user-images.githubusercontent.com/41459086/154254532-7d268e2c-87fe-4a8f-a88c-cd0109ed33dc.png)

Tambahkan remote upstream:
![image](https://user-images.githubusercontent.com/41459086/154254508-d66a6387-3904-4d04-bd7b-63acfeba176d.png)

Hasil
![image](https://user-images.githubusercontent.com/41459086/154254500-c56fde11-23ae-46ce-9ef8-8772529d609f.png)


<h3>Mengirimkan Pull Request</h3>

Setiap kali melakukan perubahan, kirim perubahan tersebut. Pengiriman ini disebut dengan Pull Request. Pada posisi ini, kontributor bisa mengirimkan kontribusi dengan cara mengirimkan pull request (PR) ke upstream author. Secara umum, langkah-langkahnya adalah sebagai berikut:

1) Kontributor akan bekerja di repo lokal (create, update, delete isi)
1) Commit
1) Push ke repo kontributor
1) Kirimkan PR ke repo upstream author.
1) Upstream author me-review dan kemudian menyetujui (merge) ke master atau menolak PR.
1) Jika disetujui dan di-merge ke repo master dari upstream author, sinkronkan repo di komputer lokal dan repo GitHub kontributor.

<h3>Membuat Perubahan di Repo Lokal</h3>

Sebelum melakukan perubahan, pastikan:

1) Sudah ada koordinasi secara manual tentang perubahan-perubahan yang akan dilakukan.
1) Setelah melakukan perubahan-perubahan, pastikan bahwa isi repo lokal tersinkronisasi dengan repo dari upstream author.
1) Cara melakukan sinkronisasi:
![image](https://user-images.githubusercontent.com/41459086/154254488-a6f17f14-7e59-44d3-8778-d83df7f12e67.png)

1) Lakukan perubahan-perubahan, setelah itu push ke origin (milik kontributor)
![image](https://user-images.githubusercontent.com/41459086/154254455-70efb899-f6a7-41e9-b121-ffc61156501d.png)
![image](https://user-images.githubusercontent.com/41459086/154254472-47a7b188-8e0c-4597-880e-fac4a6aca13a.png)

1) Setelah itu, buka halaman Web dari repo kontributor https://github.com/Riskyliana/playground. Pada halaman tersebut akan ditampilkan isi yang kita push.
![image](https://user-images.githubusercontent.com/41459086/154254428-b7f8bc6d-b1e7-4762-9c30-7c0d162c399a.png)

1) Pilih Compare and pull request, kemudian isikan deskripsi PR dan klik pada Create pull request:
![image](https://user-images.githubusercontent.com/41459086/154254405-4753f1c3-391d-4ced-91f2-5491e4fe7cc3.png)

1) Pada repo upstream author, muncul angka 1 (artinya jumlahnya 1) pada Pull requests di bagian atas.
1) Upstream author bisa menyetujui setelah melakukan review: klik pada Pull requests, akan muncul PR dengan message seperti yang ditulis oleh kontributor (Add: contributor). Klik pada PR tersebut, review kemudian klik Merge pull request diikuti dengan Confirm merge. Setelah itu, status akan berubah menjadi Merged.
1) Sinkronkan semua repo (lokal maupun GitHub kontributor)
![image](https://user-images.githubusercontent.com/41459086/154254185-d3bb3290-3eee-408f-88de-9b0bf2fa4b11.png)
![image](https://user-images.githubusercontent.com/41459086/154254140-24a4876b-8031-4bc2-83f1-fd25c9032f04.png)

<h3>Konflik</h3>

Ada kemungkinan, jika satu orang mengirimkan PR untuk satu atau lebih file dan sementara itu ada lainnya juga yang mengirimkan PR pada satu atau lebih file yang sama, maka akan terjadi konflik karena ada satu atau lebih file yang sama yang di-edit dan akan di-merge. Jika sampai terjadi kasus seperti ini, maka upatream author harus menolak semua PR dan kemudian masing-masing kontributor diharapkan menyelesaikan secara manual (offline) kemudian memutuskan siapa yang akan mengirimkan PR.
