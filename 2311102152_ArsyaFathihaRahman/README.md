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
    <strong>Arsya Fathiha Rahman</strong>
    <br>
    <strong>2311102152</strong>
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

---

# Landasan Teori

## Version Control System

Dalam proses pengembangan perangkat lunak, perubahan pada kode program sering terjadi secara berulang. Oleh karena itu diperlukan sebuah sistem yang mampu mencatat setiap perubahan tersebut sehingga riwayat pengembangan dapat diketahui dengan jelas. Sistem ini dikenal dengan istilah **Version Control System (VCS)**.

Version control membantu developer dalam melacak perubahan file, mengembalikan kode ke versi sebelumnya jika terjadi kesalahan, serta memudahkan proses kerja tim ketika beberapa orang mengerjakan proyek yang sama.

## Git

Git merupakan salah satu implementasi **version control system** yang sangat populer digunakan oleh developer di seluruh dunia. Git dikembangkan dengan tujuan agar proses pengelolaan kode program menjadi lebih terorganisir dan efisien.

Berbeda dengan sistem version control tradisional, Git menggunakan konsep **distributed system**, di mana setiap pengguna memiliki salinan lengkap dari repository beserta riwayat perubahannya. Hal ini membuat proses kolaborasi menjadi lebih fleksibel karena pekerjaan tidak bergantung pada satu server saja.

Beberapa perintah dasar Git yang sering digunakan antara lain:

- `git init` → membuat repository baru
- `git add` → menambahkan perubahan file
- `git commit` → menyimpan perubahan ke repository
- `git push` → mengirim perubahan ke repository remote
- `git pull` → mengambil perubahan dari repository remote

Dalam praktiknya Git sering digunakan bersama layanan hosting repository seperti GitHub yang menyediakan penyimpanan repository secara online.

---


## Langkah-langkah

## Langkah Pembuatan Repository Menggunakan CLI

Berikut merupakan tahapan yang dilakukan untuk membuat repository serta mengunggah tugas ke repository GitHub menggunakan Command Line Interface (CLI).

### 1. Masuk ke Folder Kerja

Langkah pertama adalah masuk ke folder kerja yang telah disiapkan sebelumnya, yaitu folder **PRAKTIKUM ABP** yang berada pada Local Disk D.

```bash
cd "/d/SEMESTER6/PRAKTIKUM ABP"
```

---

### 2. Mengunduh Repository dari GitHub

Selanjutnya mengunduh repository **modul-1** dari GitHub menggunakan perintah `git clone`.

```bash
git clone https://github.com/Aplikasi-Berbasis-Platform-S1IF-11-05/modul-1
```

Setelah proses cloning selesai, repository akan tersimpan pada folder kerja.

---

### 3. Masuk ke Folder Repository

Masuk ke dalam folder repository yang telah diunduh.

```bash
cd modul-1
```

---

### 4. Membuat Folder Tugas

Setelah berada di dalam repository, buat folder sesuai dengan format **NIM_Nama** untuk menyimpan laporan praktikum.

```bash
mkdir 2311102152_ArsyaFathihaRahman
```

Kemudian masuk ke dalam folder tersebut.

```bash
cd 2311102152_ArsyaFathihaRahman
```

---

### 5. Membuat File README

Selanjutnya membuat file **README.md** yang akan digunakan sebagai laporan praktikum.

```bash
echo "# Modul 1" > README.md
```

File README ini nantinya akan diisi dengan isi laporan praktikum.

---

### 6. Menambahkan File ke Staging Area

Setelah file README dibuat, langkah berikutnya adalah menambahkan file tersebut ke staging area menggunakan perintah berikut.

```bash
git add .
```

---

### 7. Melakukan Commit

Commit digunakan untuk menyimpan perubahan yang telah dilakukan pada repository.

```bash
git commit -m "Tugas Modul 1 - 2311102152"
```

---

### 8. Mengunggah File ke GitHub

Langkah terakhir adalah mengunggah file yang telah dibuat ke repository GitHub menggunakan perintah push.

```bash
git push origin main
```

Setelah proses push selesai, file laporan praktikum akan muncul pada repository GitHub.
