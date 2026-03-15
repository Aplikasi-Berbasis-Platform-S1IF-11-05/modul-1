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
    <strong>Retha Anggreani</strong>
    <br>
    <strong>2311102265</strong>
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

Version Control System atau VCS adalah sistem yang digunakan untuk mengelola perubahan file dalam suatu proyek. Sistem ini biasanya digunakan oleh programmer agar setiap perubahan kode dapat tercatat dengan jelas.

Dengan adanya VCS, kita bisa melihat siapa yang melakukan perubahan, kapan perubahan dilakukan, dan apa saja yang diubah pada file tersebut. Hal ini sangat membantu ketika terjadi kesalahan karena kita bisa kembali ke versi sebelumnya.

Selain itu, VCS juga memudahkan kerja tim karena beberapa orang bisa mengerjakan proyek yang sama tanpa harus takut file mereka saling tertimpa.

Terdapat dua jenis VCS yang umum digunakan:

- **Centralized Version Control System**  
  Semua data disimpan di satu server utama dan pengguna harus terhubung ke server tersebut.

- **Distributed Version Control System**  
  Setiap pengguna memiliki salinan repository lengkap di komputernya.

---

### 2. Git

Git merupakan salah satu sistem version control yang termasuk ke dalam distributed VCS. Git dibuat oleh Linus Torvalds untuk membantu proses pengembangan kernel Linux.

Saat ini Git banyak digunakan oleh developer karena mampu mengelola perubahan kode dengan baik dan mendukung kerja tim dalam satu proyek. Git juga dapat terhubung dengan berbagai layanan repository online seperti GitHub atau GitLab.

Beberapa kelebihan Git antara lain:

- Memiliki sistem pencatatan perubahan yang jelas
- Mendukung pembuatan branch untuk pengembangan fitur
- Dapat digunakan secara offline
- Mempermudah kolaborasi dalam pengembangan software

---

### 3. Struktur Penyimpanan pada Git

Dalam Git terdapat beberapa area yang digunakan untuk mengatur perubahan file, yaitu:

1. **Working Directory**  
   Merupakan tempat dimana file proyek berada dan dapat diedit oleh pengguna.

2. **Staging Area**  
   Tempat untuk menyiapkan file sebelum disimpan ke dalam commit.

3. **Repository**  
   Tempat penyimpanan permanen yang berisi semua riwayat perubahan proyek.

Dengan adanya tahapan ini, perubahan file dapat dikelola dengan lebih teratur.

---

### 4. Istilah Penting dalam Git

| Istilah | Penjelasan | Contoh Perintah |
|--------|------------|----------------|
| Repository | Tempat penyimpanan proyek yang sudah menggunakan Git | `git init` |
| Commit | Proses menyimpan perubahan ke repository | `git commit -m "pesan"` |
| Branch | Cabang pengembangan dalam proyek | `git branch` |
| Checkout | Berpindah dari satu branch ke branch lain | `git checkout` |
| Remote | Repository yang berada di server | `git remote` |
| Merge | Menggabungkan dua branch menjadi satu | `git merge` |

---

### 5. Alur Kerja Dasar Git

Berikut adalah alur dasar penggunaan Git dalam pengelolaan proyek:

1. Membuat repository baru menggunakan `git init`
2. Membuat atau mengubah file dalam proyek
3. Menambahkan file ke staging area dengan `git add`
4. Menyimpan perubahan dengan `git commit`
5. Menghubungkan repository dengan server menggunakan `git remote`
6. Mengirim perubahan ke repository online menggunakan `git push`

Dengan alur ini, setiap perubahan dalam proyek akan tercatat dengan rapi.

---

### 6. File .gitignore

Dalam Git terdapat file bernama `.gitignore` yang berfungsi untuk mengabaikan file tertentu agar tidak ikut disimpan dalam repository.

Biasanya file yang dimasukkan ke `.gitignore` adalah file sementara atau file yang tidak perlu dibagikan kepada orang lain.

Contoh isi `.gitignore`:

```
node_modules/
*.log
.env
build/
```

Dengan menggunakan `.gitignore`, repository akan lebih bersih dan hanya berisi file yang benar-benar dibutuhkan.

---

# Tugas 1
// Instalasi dan GIT

# Tugas 1
Instalasi dan Git

1. Pertama install Git dulu dari website resminya.

2. Setelah Git berhasil diinstall, buat folder baru dengan nama **APK BERBASIS PLATFORM** lalu simpan di drive D.

3. Setelah itu buka **CMD**, lalu masuk ke direktori folder yang tadi sudah dibuat.

4. Jika sudah di dalam folder tersebut, lakukan clone repository **Modul-1** dengan perintah `git clone`.

5. Setelah repository berhasil di-clone, masuk ke folder repository dengan perintah  
   `cd modul-1`.

6. Di dalam repo tersebut buat folder sesuai **NIM dan nama** dengan perintah  
   `mkdir 2311102265_RethaAnggreani`  
   lalu masuk ke foldernya dengan  
   `cd 2311102265_RethaAnggreani`.

7. Setelah itu buat file **README.md** dengan perintah  
   `echo # Modul 1 > README.md`.

8. Untuk mengedit file README.md, jalankan perintah  
   `code .`  
   supaya folder terbuka di **VS Code**.

9. Setelah selesai mengisi file README.md, kembali ke folder repo sebelumnya dengan perintah  
   `cd ..`.

10. Selanjutnya tambahkan folder dan file yang sudah dibuat ke repository dengan perintah  
    `git add .`.

11. Setelah itu buat commit dengan perintah  
    `git commit -m "Modul 1"`.

12. Sebelum melakukan push, tarik update terlebih dahulu dari repository utama dengan perintah  
    `git pull --rebase origin main`.

13. Terakhir lakukan push ke repository dengan perintah  
    `git push origin main`.

14. Jika tidak ada error berarti prosesnya sudah berhasil.
# Kesimpulan

Dari praktikum ini jadi lebih paham cara menggunakan Git sebagai version control. Mulai dari install Git, clone repository, membuat folder dan file README.md, sampai commit dan push ke repository. Dengan Git, perubahan file dalam proyek bisa tercatat dengan rapi dan lebih mudah dikelola.