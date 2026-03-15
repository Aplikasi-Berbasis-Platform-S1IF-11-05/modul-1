<div align="center">
  <br />
  <h1>LAPORAN PRAKTIKUM <br> APLIKASI BERBASIS PLATFORM </h1>
  <br />
  <h3>MODUL 1 <br> Instalasi dan GIT </h3>
  <br />
  <img width="512" height="512" alt="telyu" src="https://github.com/user-attachments/assets/724a3291-bcf9-448d-a395-3886a8659d79" />
  <br />
  <br />
  <br />
  <h3>Disusun Oleh :</h3>
  <p>
    <strong>Muhamad Rafli Al Farizqi</strong>
    <br>
    <strong>2311102315</strong>
    <br>
    <strong>S1 IF-11-REG05</strong>
  </p>
  <br />
  <h3>Dosen Pengampu :</h3>
  <p>
    <strong>Dedi Agung Prabowo, S.Kom., M.Kom</strong>
  </p>
  <br />
  <br />
  <h4>Asisten Praktikum :</h4>
  <strong>Apri Pandu Wicaksono </strong>
  <br>
  <strong>Hamka Zaenul Ardi</strong>
  <br />
  <h3>LABORATORIUM HIGH PERFORMANCE <br>FAKULTAS INFORMATIKA <br>UNIVERSITAS TELKOM PURWOKERTO <br>2026 </h3>
</div>

<hr>

# Dasar Teori

### 1. Version Control System (VCS)

Version Control System (VCS) adalah sebuah sistem yang mencatat setiap perubahan pada file atau kumpulan file dari waktu ke waktu sehingga pengguna dapat mengakses kembali versi tertentu di kemudian hari. VCS sangat penting dalam pengembangan perangkat lunak karena memungkinkan pelacakan perubahan kode secara sistematis.

Manfaat utama dari VCS antara lain:
- Mencatat seluruh riwayat perubahan file beserta informasi siapa yang mengubah dan kapan perubahan dilakukan
- Memungkinkan pengembalian ke versi sebelumnya apabila terjadi kesalahan
- Mendukung kolaborasi antar anggota tim tanpa risiko file saling tertimpa

Terdapat dua jenis utama VCS:

- **Centralized Version Control System (CVCS)**
  Pada sistem ini, seluruh riwayat perubahan tersimpan di satu server pusat. Pengguna harus terhubung ke server untuk mengakses dan menyimpan perubahan. Contoh: SVN, CVS.

- **Distributed Version Control System (DVCS)**
  Setiap pengguna memiliki salinan lengkap dari repository di komputernya masing-masing, sehingga bisa bekerja secara offline. Contoh: Git, Mercurial.

---

### 2. Git

Git adalah sistem version control terdistribusi (DVCS) yang diciptakan oleh Linus Torvalds pada tahun 2005 untuk mendukung pengembangan kernel Linux. Git dirancang agar cepat, efisien, dan mampu menangani proyek berskala besar.

Git saat ini menjadi tools version control paling populer di kalangan developer karena kemampuannya dalam mengelola perubahan kode secara efektif. Git dapat diintegrasikan dengan platform repository online seperti GitHub, GitLab, dan Bitbucket.

Beberapa kelebihan Git:

- Memiliki performa yang cepat dalam melakukan operasi seperti commit, merge, dan branching
- Mendukung pengembangan paralel melalui fitur branching
- Bisa digunakan secara offline karena setiap pengguna memiliki salinan repository lengkap
- Mempermudah kolaborasi tim dalam pengembangan perangkat lunak
- Memiliki integritas data yang tinggi menggunakan SHA-1 hash

---

### 3. Struktur Penyimpanan pada Git

Git memiliki tiga area utama dalam mengelola perubahan file:

1. **Working Directory**
   Area kerja dimana file proyek berada. Di sinilah pengguna melakukan perubahan pada file-file proyek.

2. **Staging Area (Index)**
   Area perantara yang digunakan untuk menandai file mana saja yang akan dimasukkan ke dalam commit berikutnya. File ditambahkan ke staging area menggunakan perintah `git add`.

3. **Repository (.git directory)**
   Tempat penyimpanan permanen yang menyimpan seluruh metadata dan riwayat perubahan proyek. Setiap commit akan tersimpan di dalam repository ini.

Alur perpindahan file: Working Directory → Staging Area → Repository

---

### 4. Istilah Penting dalam Git

| Istilah | Penjelasan | Contoh Perintah |
|--------|------------|----------------|
| Repository | Tempat penyimpanan proyek beserta riwayat perubahannya | `git init` |
| Clone | Menyalin repository dari remote ke lokal | `git clone <url>` |
| Commit | Menyimpan snapshot perubahan ke repository lokal | `git commit -m "pesan"` |
| Branch | Cabang pengembangan independen dalam proyek | `git branch <nama>` |
| Checkout | Berpindah ke branch atau commit tertentu | `git checkout <branch>` |
| Remote | Repository yang berada di server (GitHub/GitLab) | `git remote add origin <url>` |
| Merge | Menggabungkan perubahan dari satu branch ke branch lain | `git merge <branch>` |
| Push | Mengirim commit lokal ke remote repository | `git push origin main` |
| Pull | Mengambil dan menggabungkan perubahan dari remote | `git pull origin main` |

---

### 5. Alur Kerja Dasar Git

Berikut adalah langkah-langkah dasar dalam menggunakan Git untuk mengelola proyek:

1. Inisialisasi repository baru dengan `git init` atau clone repository yang sudah ada dengan `git clone`
2. Membuat atau memodifikasi file di dalam working directory
3. Menambahkan file yang telah diubah ke staging area menggunakan `git add`
4. Menyimpan perubahan secara permanen ke repository dengan `git commit`
5. Menghubungkan repository lokal dengan remote repository menggunakan `git remote add`
6. Mengirim perubahan ke remote repository menggunakan `git push`

Dengan mengikuti alur ini, setiap perubahan dalam proyek akan terdokumentasi dengan baik dan dapat dilacak kapan saja.

---

### 6. File .gitignore

File `.gitignore` adalah file konfigurasi yang memberitahu Git file atau direktori mana yang harus diabaikan dan tidak perlu dilacak perubahannya. File ini sangat berguna untuk mengecualikan file-file yang tidak relevan dari repository.

File yang umumnya dimasukkan ke `.gitignore`:
- Folder dependencies seperti `node_modules/`
- File environment seperti `.env`
- File hasil build atau kompilasi
- File log dan file sementara

Contoh isi `.gitignore`:

```
node_modules/
*.log
.env
build/
dist/
.DS_Store
```

Dengan `.gitignore`, repository tetap bersih dan hanya berisi file source code yang memang diperlukan.

---

# Tugas 1

Instalasi dan Git

1. Langkah pertama adalah menginstall Git dari website resminya di [git-scm.com](https://git-scm.com/).

2. Setelah Git terinstall, buat folder baru untuk menyimpan proyek praktikum.

3. Buka **Terminal** atau **CMD**, lalu navigasi ke direktori folder yang sudah dibuat.

4. Clone repository **Modul-1** dari GitHub menggunakan perintah `git clone`.

5. Masuk ke folder repository yang sudah di-clone dengan perintah
   `cd modul-1`.

6. Buat folder sesuai NIM dan nama dengan perintah
   `mkdir 2311102315_MuhamadRafliAlFarizqi`
   lalu masuk ke folder tersebut dengan
   `cd 2311102315_MuhamadRafliAlFarizqi`.

7. Buat file **README.md** dengan perintah
   `echo # Modul 1 > README.md`.

8. Edit file README.md menggunakan text editor, bisa dengan menjalankan
   `code .`
   untuk membuka folder di **VS Code**.

9. Setelah selesai mengedit README.md, kembali ke folder repository utama dengan
   `cd ..`.

10. Tambahkan semua perubahan ke staging area dengan perintah
    `git add .`.

11. Buat commit untuk menyimpan perubahan dengan perintah
    `git commit -m "Modul 1"`.

12. Sebelum push, lakukan pull terlebih dahulu untuk sinkronisasi dengan remote repository
    `git pull --rebase origin main`.

13. Push perubahan ke remote repository dengan perintah
    `git push origin main`.

14. Jika tidak ada error, maka proses sudah berhasil.

# Kesimpulan

Dari praktikum Modul 1 ini, dapat disimpulkan bahwa Git merupakan tools version control yang sangat penting dalam pengembangan perangkat lunak. Melalui praktikum ini, saya mempelajari cara menginstall Git, melakukan clone repository, membuat folder dan file README.md, serta melakukan commit dan push ke remote repository. Git memungkinkan setiap perubahan dalam proyek tercatat secara sistematis sehingga memudahkan pengelolaan dan kolaborasi dalam pengembangan software.
