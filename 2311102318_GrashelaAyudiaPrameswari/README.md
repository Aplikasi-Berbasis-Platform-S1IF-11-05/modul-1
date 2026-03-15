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
    <strong>Grashela Ayudia Prameswari</strong>
    <br>
    <strong>2311102318</strong>
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

Version Control System (VCS) merupakan sebuah sistem yang digunakan untuk mencatat dan mengelola setiap perubahan yang terjadi pada file dalam suatu proyek. Sistem ini sangat penting dalam pengembangan perangkat lunak karena memungkinkan pengembang untuk melacak siapa yang melakukan perubahan, kapan perubahan tersebut dilakukan, serta apa saja yang berubah dari versi sebelumnya.

Dengan adanya VCS, pengembang dapat dengan mudah kembali ke versi sebelumnya apabila terjadi kesalahan. Selain itu, VCS juga mendukung kolaborasi tim sehingga beberapa orang dapat bekerja pada proyek yang sama secara bersamaan tanpa khawatir saling menimpa pekerjaan satu sama lain.

Terdapat dua jenis utama VCS yang umum digunakan:

- **Centralized Version Control System (CVCS)**
  Pada sistem ini, seluruh data dan riwayat perubahan disimpan di satu server pusat. Pengguna harus terhubung ke server tersebut untuk mengakses dan melakukan perubahan pada proyek.

- **Distributed Version Control System (DVCS)**
  Setiap pengguna memiliki salinan lengkap dari repository di komputernya masing-masing, sehingga pekerjaan tetap dapat dilakukan secara offline.

---

### 2. Git

Git adalah sistem pengontrol versi terdistribusi (Distributed Version Control System) yang diciptakan oleh Linus Torvalds pada tahun 2005. Awalnya Git dikembangkan untuk mendukung proses pengembangan kernel Linux, namun saat ini Git telah menjadi salah satu tools yang paling banyak digunakan oleh developer di seluruh dunia.

Git memiliki kemampuan untuk mengelola perubahan kode secara efisien dan mendukung kolaborasi dalam tim pengembangan perangkat lunak. Git juga dapat dihubungkan dengan berbagai layanan repository online seperti GitHub, GitLab, dan Bitbucket.

Beberapa kelebihan Git antara lain:

- Memiliki sistem pencatatan perubahan yang detail dan jelas
- Mendukung pembuatan branch untuk pengembangan fitur secara terpisah
- Dapat digunakan secara offline tanpa memerlukan koneksi internet
- Mempermudah proses kolaborasi antar anggota tim
- Memiliki performa yang cepat dalam mengelola repository

---

### 3. Struktur Penyimpanan pada Git

Git memiliki tiga area utama dalam mengelola perubahan file:

1. **Working Directory**
   Merupakan area kerja dimana file-file proyek berada dan dapat diedit secara langsung oleh pengguna.

2. **Staging Area (Index)**
   Area sementara yang digunakan untuk menyiapkan file-file yang akan disimpan ke dalam commit. File yang sudah ditambahkan ke staging area siap untuk di-commit.

3. **Repository**
   Tempat penyimpanan permanen yang berisi seluruh riwayat perubahan proyek. Setiap commit yang dilakukan akan tersimpan di repository ini.

---

### 4. Istilah Penting dalam Git

| Istilah    | Penjelasan                                          | Contoh Perintah                |
|------------|-----------------------------------------------------|--------------------------------|
| Repository | Tempat penyimpanan proyek yang dikelola oleh Git    | `git init`                     |
| Clone      | Menyalin repository dari server ke komputer lokal   | `git clone <url>`              |
| Commit     | Menyimpan perubahan ke dalam repository              | `git commit -m "pesan"`        |
| Branch     | Cabang pengembangan dalam sebuah proyek              | `git branch <nama-branch>`     |
| Checkout   | Berpindah dari satu branch ke branch lain            | `git checkout <nama-branch>`   |
| Merge      | Menggabungkan dua branch menjadi satu                | `git merge <nama-branch>`      |
| Push       | Mengirim perubahan dari lokal ke repository remote   | `git push origin main`         |
| Pull       | Mengambil perubahan terbaru dari repository remote   | `git pull origin main`         |
| Remote     | Repository yang berada di server (misalnya GitHub)   | `git remote add origin <url>`  |

---

### 5. Alur Kerja Dasar Git

Berikut adalah alur dasar penggunaan Git dalam pengelolaan proyek:

1. Membuat repository baru menggunakan `git init` atau melakukan clone dari repository yang sudah ada dengan `git clone`
2. Membuat atau mengubah file di dalam working directory
3. Menambahkan file yang telah diubah ke staging area menggunakan `git add`
4. Menyimpan perubahan secara permanen dengan `git commit`
5. Menghubungkan repository lokal dengan repository online menggunakan `git remote add origin`
6. Mengirim perubahan ke repository online menggunakan `git push`

---

### 6. File .gitignore

File `.gitignore` adalah file khusus dalam Git yang berfungsi untuk menentukan file atau folder mana saja yang tidak perlu dilacak oleh Git. File ini berguna untuk mengabaikan file-file sementara, file konfigurasi lokal, atau file hasil build yang tidak perlu disimpan di repository.

Contoh isi file `.gitignore`:

```
node_modules/
*.log
.env
build/
.DS_Store
```

Dengan menggunakan `.gitignore`, repository akan tetap bersih dan hanya berisi file-file yang benar-benar dibutuhkan dalam proyek.

---

# Tugas 1

Instalasi dan Git

1. Langkah pertama adalah mengunduh dan menginstall Git dari website resmi Git di https://git-scm.com/.

2. Setelah Git berhasil terinstall, buka **Command Prompt (CMD)** dan pastikan Git sudah terpasang dengan benar menggunakan perintah:
   ```
   git --version
   ```

3. Lakukan konfigurasi awal Git dengan mengatur username dan email:
   ```
   git config --global user.name "Grashela Ayudia Prameswari"
   git config --global user.email "grashela@students.telkomuniversity.ac.id"
   ```

4. Buat folder baru untuk menyimpan proyek praktikum, kemudian masuk ke direktori folder tersebut melalui CMD.

5. Lakukan clone repository **Modul-1** menggunakan perintah:
   ```
   git clone <url-repository>
   ```

6. Setelah repository berhasil di-clone, masuk ke folder repository dengan perintah:
   ```
   cd modul-1
   ```

7. Di dalam repository, buat folder sesuai NIM dan nama menggunakan perintah:
   ```
   mkdir 2311102318_GrashelaAyudiaPrameswari
   ```
   Kemudian masuk ke folder tersebut:
   ```
   cd 2311102318_GrashelaAyudiaPrameswari
   ```

8. Buat file **README.md** dengan perintah:
   ```
   echo # Modul 1 > README.md
   ```

9. Untuk mengedit file README.md, buka folder di **VS Code** dengan perintah:
   ```
   code .
   ```

10. Setelah selesai mengedit file README.md, kembali ke folder repository:
    ```
    cd ..
    ```

11. Tambahkan semua file yang sudah dibuat ke staging area:
    ```
    git add .
    ```

12. Buat commit untuk menyimpan perubahan:
    ```
    git commit -m "menambahkan laporan modul 1 Grashela Ayudia Prameswari"
    ```

13. Sebelum melakukan push, tarik update terlebih dahulu dari repository utama:
    ```
    git pull --rebase origin main
    ```

14. Terakhir, kirim perubahan ke repository online:
    ```
    git push origin main
    ```

15. Jika tidak ada error, maka proses sudah berhasil dan file telah terunggah ke GitHub.

---

# Kesimpulan

Dari praktikum Modul 1 ini, dapat disimpulkan bahwa Git merupakan tools yang sangat penting dalam pengembangan perangkat lunak. Git memungkinkan pengembang untuk mencatat setiap perubahan yang terjadi pada file proyek secara terstruktur dan rapi. Melalui praktikum ini, telah dipelajari cara menginstall Git, melakukan konfigurasi awal, membuat repository, serta melakukan operasi dasar Git seperti clone, add, commit, dan push. Pemahaman tentang Git dan GitHub sangat diperlukan untuk mendukung proses kolaborasi dalam pengembangan proyek perangkat lunak secara efisien.
