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
    <strong>MUHAMMAD AULIA MUZZAKI NUGRAHA</strong>
    <br>
    <strong>2311102051</strong>
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

Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.
Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.
Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.

# Task 1: Pemanasan Terminal
Setup repository-nya wajib via CLI ya. Simpen dulu mouse lu, biasain ngetik command biar kelihatan kayak hacker beneran. [aku heker kata mamah]

## Install Git
![Install Git](assets/installGit.png)

## Step Pembuatan Repository Pribadi (Via CLI Git)

1. Buka terminal, lalu masuk ke folder kerja.

```bash
cd "C:\Users\M S I\Pictures\apalah"
```
![Buka Terminal](assets/step1.png)

2. Masuk ke folder proyek kamu.

```bash
mkdir modul-1
cd modul-1
```
![Membuat folder](assets/step2.png)

3. Lalu inisialisasi Git, hubungkan folder lokal ke repository GitHub pribadi.

```bash
git init
git remote add origin https://github.com/aelyn4k/modul-1test.git
```
![Menghubungkan folder lokal dengan repository github](assets/step3.png)

4. Cek status dan branch aktif.

```bash
git status
git branch
```
![cek status dan branch aktif](assets/step4.png)

5. Buat atau edit file laporan pada folder masing-masing.

```bash
echo "Zaki" >> README.md
```
![Membuat file](assets/step5.png)

6. Tambahkan perubahan ke staging area.

```bash
git add .
```
![Perubahan ke staging area](assets/step6.png)

7. Commit perubahan.

```bash
git commit -m "Ini tugas modul 1"
```
![Commit perubahan](assets/step7.png)

8. Pastikan branch utama bernama `main`.

```bash
git branch -M main
```
![memastikan branch main](assets/step8.png)

9. Push hasil commit pertama ke GitHub pribadi.

```bash
git push -u origin main
```
![push ke github](assets/step9(1).png)
![push ke github](assets/step9(2).png)

