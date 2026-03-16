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
    <strong>Buswiryawan Raditya Boenyamin</strong>
    <br>
    <strong>2311102090</strong>
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
Git ialah salah  satu sistem pengontrol versi (Version Control System) di proyek aplikasi yg
diciptakan oleh Linus Torvalds. Pengontrol versi bertugas mencatat setiap perubahan pada arsip proyek yg
dikerjakan oleh banyak orang juga sendiri. Git dikenal pula menggunakan distributed revision control (VCS
terdistribusi), merupakan penyimpanan database Git tidak hanya berada dalam satu tempat saja.

# Tugas 1
Setup repository-nya wajib via CLI ya. Simpen dulu mouse lu, biasain ngetik command biar kelihatan kayak hacker beneran.
```bash
# 1. Konfigurasi identitas Git (lakukan sekali saja)
git config --global user.name "Buswiryawan Raditya Boenyamin"
git config --global user.email "email@example.com"
 
# 2. Buat folder proyek dan masuk ke dalamnya
mkdir modul-1-git
cd modul-1-git
 
# 3. Inisialisasi repositori Git baru
git init
 
# 4. Buat file pertama
touch README.md
echo "# Modul 1 - Git" >> README.md
 
# 5. Cek status perubahan
git status
 
# 6. Tambahkan file ke staging area
git add README.md
 
# 7. Commit perubahan
git commit -m "first commit"
 
# 8. Hubungkan ke repositori GitHub
git remote add origin https://github.com/Buswir/modul-1-git.git
 
# 9. Push ke GitHub
git push -u origin master

```
Output:
<img width="1901" height="961" alt="image" src="Output/Screenshot 2026-03-16 173151.png" />

