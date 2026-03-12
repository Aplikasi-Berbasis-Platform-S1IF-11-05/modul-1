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
<img width="848" height="192" alt="masuk folder" src="https://github.com/user-attachments/assets/a9588321-23cb-4f4f-97a4-388128a6a6b8" />


---

### 2. Mengunduh Repository dari GitHub

Selanjutnya mengunduh repository **modul-1** dari GitHub menggunakan perintah `git clone`.

```bash
git clone https://github.com/Aplikasi-Berbasis-Platform-S1IF-11-05/modul-1
```

Setelah proses cloning selesai, repository akan tersimpan pada folder kerja.
<img width="830" height="171" alt="github" src="https://github.com/user-attachments/assets/56526f74-0853-4362-8cd7-8d4af8724126" />


---

### 3. Masuk ke Folder Repository

Masuk ke dalam folder repository yang telah diunduh.

```bash
cd modul-1
```
<img width="413" height="58" alt="cd modul" src="https://github.com/user-attachments/assets/0309a242-ff9b-4bec-b841-057a3b2aa222" />

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
<img width="583" height="105" alt="mkdir " src="https://github.com/user-attachments/assets/e9424ab4-db6f-4b65-9c3b-7b23edfcb5c1" />

---

### 5. Membuat File README

Selanjutnya membuat file **README.md** yang akan digunakan sebagai laporan praktikum.

```bash
echo "# Modul 1" > README.md
```

File README ini nantinya akan diisi dengan isi laporan praktikum.
<img width="786" height="120" alt="file readme" src="https://github.com/user-attachments/assets/e2467ff7-7dd2-4579-98e6-76507859b102" />

---

### 6. Menambahkan File ke Staging Area

Setelah file README dibuat, langkah berikutnya adalah menambahkan file tersebut ke staging area menggunakan perintah berikut.

```bash
git add .
```
<img width="739" height="120" alt="git add" src="https://github.com/user-attachments/assets/caafd9c4-cc23-4006-bb34-7be03e13ea57" />

---

### 7. Melakukan Commit

Commit digunakan untuk menyimpan perubahan yang telah dilakukan pada repository.

```bash
git commit -m "Tugas Modul 1 - 2311102152"
```
<img width="751" height="128" alt="commit" src="https://github.com/user-attachments/assets/27f54695-e37d-4461-923a-3f4ad29a7c0f" />

---

### 8. Mengunggah File ke GitHub

Langkah terakhir adalah mengunggah file yang telah dibuat ke repository GitHub menggunakan perintah push.

```bash
git push origin main
```
<img width="823" height="267" alt="push" src="https://github.com/user-attachments/assets/5622c030-6905-44e9-b65d-d7a14c9ff19a" />

Setelah proses push selesai, file laporan praktikum akan muncul pada repository GitHub.

---

## Hasil Program

Berikut adalah hasil dari proses praktikum yang telah dilakukan menggunakan Git melalui Command Line Interface. Pada tahap ini seluruh langkah mulai dari proses cloning repository, pembuatan folder tugas, pembuatan file README, hingga proses commit dan push ke GitHub telah berhasil dilakukan.

<img width="1920" height="1080" alt="2311102152_Git" src="https://github.com/user-attachments/assets/fa1ae61c-b7c9-4310-9634-2c9b3884923b" />


Berikut adalah beberapa hasil tampilan dari proses yang telah dilakukan:
<img width="1920" height="1080" alt="Arsya_Hasil tampilan" src="https://github.com/user-attachments/assets/de441fb0-32cc-4c2d-9c16-06eed83ee249" />



---

## Kesimpulan

Berdasarkan praktikum yang telah dilakukan, dapat disimpulkan bahwa Git merupakan salah satu sistem version control yang sangat penting dalam proses pengembangan perangkat lunak. Dengan menggunakan Git, setiap perubahan pada proyek dapat tercatat dengan baik sehingga memudahkan pengelolaan kode program.

Selain itu, penggunaan Git juga mempermudah proses kolaborasi antar developer karena setiap orang dapat bekerja pada repository yang sama tanpa harus khawatir kehilangan perubahan yang telah dibuat. Melalui praktikum ini, mahasiswa dapat memahami dasar penggunaan Git seperti melakukan clone repository, menambahkan file ke staging area, melakukan commit, serta mengunggah perubahan ke repository GitHub.
