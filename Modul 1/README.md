# Anisah Syifa Mustika Riyanto

# 2311102080

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
    <strong>Anisah Syifa Mustika Riyanto</strong>
    <br>
    <strong>2311102080</strong>
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

Pengertian Git

Git adalah sistem pengontrol versi (Version Control System) yang dibuat oleh Linus Torvalds pada tahun 2005. Git digunakan untuk mencatat setiap perubahan yang terjadi pada file dalam sebuah proyek, terutama proyek perangkat lunak. Dengan menggunakan Git, setiap perubahan yang dilakukan dapat disimpan dan dilacak sehingga memudahkan pengembang dalam mengelola perkembangan proyek.

Git bersifat terdistribusi, artinya setiap pengguna yang bekerja dalam sebuah proyek memiliki salinan lengkap dari seluruh data proyek. Hal ini membuat proses pengembangan menjadi lebih aman dan fleksibel, karena data proyek tidak hanya tersimpan di satu tempat saja. Melalui Git, pengguna dapat melihat riwayat perubahan file, mengetahui siapa yang melakukan perubahan, serta mengembalikan file ke versi sebelumnya apabila terjadi kesalahan.

Fungsi Git dalam Kolaborasi Proyek

Git sangat membantu dalam proses kolaborasi tim ketika mengembangkan sebuah proyek. Beberapa orang dapat bekerja pada proyek yang sama secara bersamaan tanpa saling mengganggu pekerjaan masing-masing. Hal ini dimungkinkan karena Git memiliki fitur branching dan merging.

Fitur branching memungkinkan pengembang membuat cabang baru dari proyek utama untuk mengembangkan fitur tertentu atau memperbaiki kesalahan. Setelah pekerjaan selesai dan dianggap stabil, perubahan tersebut dapat digabungkan kembali ke cabang utama melalui proses yang disebut merging. Dengan cara ini, pengembangan proyek dapat dilakukan secara lebih terorganisir dan efisien.

GitHub sebagai Platform Pendukung Git

Dalam praktiknya, Git sering digunakan bersama dengan platform berbasis web seperti GitHub. GitHub berfungsi sebagai layanan penyimpanan repository Git secara online yang memungkinkan pengguna menyimpan proyek di cloud serta membagikan kode kepada orang lain.

Melalui GitHub, pengguna dapat berkolaborasi dengan tim secara lebih mudah karena semua anggota dapat mengakses repository yang sama melalui internet. Selain itu, GitHub juga menyediakan berbagai fitur tambahan seperti pelacakan perubahan, manajemen proyek, serta sistem diskusi yang membantu proses pengembangan perangkat lunak menjadi lebih terstruktur.

Penggunaan Git melalui Command Line Interface (CLI)

Git dapat digunakan melalui Command Line Interface (CLI), yaitu antarmuka berbasis teks yang dijalankan melalui terminal atau command prompt. Dengan CLI, pengguna dapat menjalankan berbagai perintah Git secara langsung dengan mengetikkan perintah tertentu.

Beberapa operasi dasar yang dapat dilakukan melalui CLI antara lain membuat repository, menambahkan file ke dalam repositori, melakukan commit untuk menyimpan perubahan, serta mengirimkan perubahan tersebut ke repository yang ada di GitHub. Penggunaan CLI membantu pengguna memahami cara kerja Git secara lebih mendalam karena setiap proses dilakukan secara manual melalui terminal.

Kesimpulan

Secara keseluruhan, Git merupakan alat yang sangat penting dalam pengembangan perangkat lunak modern. Dengan kemampuannya dalam mencatat perubahan, mengelola versi file, serta mendukung kolaborasi tim, Git membantu pengembang bekerja secara lebih terstruktur dan efisien. Dukungan platform seperti GitHub serta penggunaan melalui CLI semakin memudahkan proses pengelolaan proyek perangkat lunak.

# Tugas 1

```
//2311102080
//Anisah Syifa Mustika Riyanto

## Proses Pengerjaan Tugas

1. Memastikan aplikasi Git telah terpasang pada komputer dengan menjalankan perintah berikut pada Windows PowerShell:

```

git --version

```

Perintah tersebut digunakan untuk mengecek versi Git yang terinstall pada sistem.

2. Mengarahkan direktori kerja ke folder penyimpanan praktikum yang berada pada Local Disk D dengan menggunakan perintah:

```

cd "D:\Huru-Hara Semester 6\Aplikasi Berbasis Platform\Praktikum"

```

Perintah `cd` digunakan untuk berpindah direktori ke lokasi folder tempat penyimpanan file praktikum.

3. Membuat repository Git baru pada folder tersebut dengan menjalankan perintah:

```

git init

```

Perintah ini berfungsi untuk menginisialisasi repository Git sehingga folder praktikum dapat dikelola menggunakan Git.

4. Menghubungkan repository lokal dengan repository yang ada di platform GitHub menggunakan perintah:

```

git remote add origin https://github.com/zephyrmr/Praktikum-ABP.git

```

Langkah ini bertujuan agar repository lokal dapat terhubung dengan repository online sehingga file dapat diunggah ke GitHub.

5. Membuat struktur folder untuk setiap modul praktikum menggunakan perintah:

```

mkdir "Modul 1"
mkdir "Modul 2"

```

Perintah `mkdir` digunakan untuk membuat direktori baru sebagai tempat penyimpanan laporan masing-masing modul.

6. Menambahkan seluruh file yang terdapat dalam folder praktikum ke dalam staging area Git menggunakan perintah:

```

git add .

```

Perintah ini digunakan untuk memasukkan semua file yang ada dalam folder ke dalam proses pelacakan Git.

7. Melakukan penyimpanan perubahan menggunakan perintah commit:

```

git commit -m "first commit"

```

Pada tahap ini sempat terjadi pesan kesalahan karena identitas pengguna Git (username dan email) belum dikonfigurasi.

8. Mengatur konfigurasi identitas pengguna Git dengan menjalankan perintah berikut:

```

git config --global user.email "asyifaa21405@gmail.com"
git config --global user.name "zephyrmr"

```

Konfigurasi ini diperlukan agar Git dapat mencatat siapa yang melakukan perubahan pada repository.

9. Setelah konfigurasi berhasil dilakukan, proses commit dijalankan kembali untuk menyimpan perubahan yang telah dilakukan pada repository lokal.

```

Output:
<img width="1901" height="961" alt="image" src="Git.png" />
