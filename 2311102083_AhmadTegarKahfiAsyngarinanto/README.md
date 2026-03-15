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
    <strong>Ahmad Tegar Kahfi Asyngarinanto</strong>
    <br>
    <strong>2311102083</strong>
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
  <strong>Apri Pandu Wicaksono</strong>
  <br>
  <strong>Hamka Zaenul Ardi</strong>
  <br />
  <h3>LABORATORIUM HIGH PERFORMANCE <br>FAKULTAS INFORMATIKA <br>UNIVERSITAS TELKOM PURWOKERTO <br>2026 </h3>
</div>

<hr>

# Dasar Teori

## 1. Git

Git adalah sistem kontrol versi terdistribusi (*distributed version control system*) yang digunakan untuk melacak perubahan pada file atau kumpulan file dari waktu ke waktu. Git dikembangkan oleh Linus Torvalds pada tahun 2005 dan kini menjadi salah satu alat paling populer dalam pengembangan perangkat lunak.

Dengan Git, setiap developer memiliki salinan penuh dari seluruh riwayat proyek di komputer lokal mereka, sehingga memungkinkan pengembangan yang cepat, aman, dan dapat dilacak. Git mendukung alur kerja non-linear melalui cabang (*branching*) dan penggabungan (*merging*) yang sangat fleksibel.

**Konsep Utama Git:**
- **Repository (Repo):** Tempat penyimpanan proyek beserta seluruh riwayat perubahannya.
- **Commit:** Rekaman snapshot dari perubahan yang telah dilakukan.
- **Branch:** Cabang pengembangan yang memungkinkan pekerjaan paralel.
- **Staging Area:** Area antara di mana perubahan disiapkan sebelum di-commit.
- **Working Directory:** Direktori lokal tempat kita bekerja dan mengubah file.

**Perintah Dasar Git:**

| Perintah | Fungsi |
|----------|--------|
| `git init` | Menginisialisasi repositori Git baru |
| `git clone <url>` | Menyalin repositori dari remote |
| `git add <file>` | Menambahkan file ke staging area |
| `git commit -m "pesan"` | Menyimpan perubahan dengan pesan |
| `git push` | Mengirim commit ke remote repository |
| `git pull` | Mengambil dan menggabungkan perubahan dari remote |
| `git status` | Melihat status perubahan file |
| `git log` | Melihat riwayat commit |

---

## 2. GitHub

GitHub adalah platform hosting berbasis cloud untuk repositori Git. GitHub menyediakan antarmuka web yang memudahkan kolaborasi antar developer, manajemen proyek, dan penyimpanan kode sumber secara online. GitHub menggunakan Git sebagai sistem kontrol versi di baliknya.

**Fitur Utama GitHub:**
- **Repository:** Tempat menyimpan dan mengelola kode proyek secara online.
- **Commit History:** Melacak semua perubahan yang telah dilakukan pada kode.
- **Pull Request:** Mekanisme untuk mengajukan perubahan agar ditinjau dan digabungkan.
- **Issues:** Sistem pelacak bug dan diskusi fitur.
- **README.md:** File dokumentasi utama yang ditampilkan di halaman repository.

---

## 3. Hubungan Git dan GitHub

Git adalah *tool* yang berjalan di komputer lokal untuk mengelola versi file, sedangkan GitHub adalah layanan *cloud* yang menjadi tempat penyimpanan remote dari repositori Git. Keduanya bekerja bersama: Git digunakan untuk membuat dan mengelola commit secara lokal, lalu hasilnya di-*push* ke GitHub agar dapat diakses dan dibagikan kepada orang lain.

---

# Tugas 1

## Langkah-Langkah Upload Tugas ke GitHub via Git (Windows)

### Prasyarat
Pastikan Git sudah terinstal di komputer. Cek dengan membuka **Git Bash** atau **Command Prompt** dan ketik:
```
git --version
```
Jika muncul versi Git, berarti Git sudah siap digunakan.

---

### Langkah 1 – Clone Repository Tugas

Buka **Git Bash**, lalu clone repository mata kuliah ke komputer lokal. Pindah terlebih dahulu ke direktori yang diinginkan.
```bash
cd Desktop
git clone https://github.com/Aplikasi-Berbasis-Platform-S1IF-11-05/modul-1
cd modul-1
```

---

### Langkah 2 – Buat Folder dengan Format NIM_Nama

Di dalam folder hasil clone, buat folder baru dengan format **NIM_NamaLengkap**:

```bash
mkdir "2311102083_AhmadTegarKahfiAsyngarinanto"
```

---

### Langkah 3 – Masuk ke Folder yang Sudah Dibuat

```bash
cd "2311102083_AhmadTegarKahfiAsyngarinanto"
```

---

### Langkah 4 – Buat File README.md

Buat file README.md di dalam folder tersebut:

```bash
echo "" >> README.md
```

Kemudian buka file `README.md` menggunakan teks editor (misalnya VS Code atau Notepad), lalu isi dengan laporan praktikum sesuai format yang telah ditentukan (seperti laporan ini).

---

### Langkah 5 – Kembali ke Root Repository

Setelah selesai mengisi README.md, kembali ke folder utama repository:

```bash
cd ..
```

---

### Langkah 6 – Cek Status Perubahan

Lihat file apa saja yang berubah atau baru ditambahkan:

```bash
git status
```

Akan muncul folder/file baru yang ditandai sebagai *untracked* (belum dilacak Git).

---

### Langkah 7 – Tambahkan Perubahan ke Staging Area

Tambahkan folder beserta isinya ke staging area:

```bash
git add "2311102083_AhmadTegarKahfiAsyngarinanto"
```

Atau tambahkan semua perubahan sekaligus:

```bash
git add .
```

---

### Langkah 8 – Commit Perubahan

Simpan perubahan dengan pesan commit yang jelas:

```bash
git commit -m "Tugas Modul 1 - Instalasi & Git"
```

---

### Langkah 9 – Push ke GitHub

Kirim commit ke repository GitHub:

```bash
git push
```


---

### Langkah 10 – Verifikasi di GitHub

Buka browser dan kunjungi URL repository:
```
https://github.com/Aplikasi-Berbasis-Platform-S1IF-11-05/modul-1
```
Pastikan folder `2311102083_AhmadTegarKahfiAsyngarinanto` sudah muncul di halaman repository. ✅

---

## Output

```
//2311102083
//Ahmad Tegar Kahfi Asyngarinanto

<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Aku Cinta Telkom</title>
</head>
<body>
  ...
</body>
</html>
```

Output:

![Bukti](Assets/Bukti.png)
