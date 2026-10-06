# Telkom University Company Profile - Praktikum

Proyek simulasi untuk mempelajari HTML, CSS, PHP native, MySQL/MariaDB, dan Git.

## Menjalankan secara lokal
1. Salin folder proyek ke `C:\xampp\htdocs\`.
2. Start Apache dan MySQL di XAMPP.
3. Import `database/telkom_profile.sql` melalui phpMyAdmin.
4. Buka `http://localhost/telkom-company-profile/`.


## Penyelesaian Merge Conflict 
pada Bab 12 Conflict dibuat secara sengaja dengan mengubah menu "Profil" di `includes/header.php` pada dua branch:

`main` menjadi "Tentang Kampus", sedangkan `conflict-navbar` menjadi "Tentang Kami".
Saat `git merge conflict-navbar`, Git menampilkan conflict karena kedua branch mengubah baris yang sama.

Penyelesaian: memilih teks final "Profil", menghapus marker `<<<<<<<`, `=======`, dan `>>>>>>>`,
menjalankan `git add includes/header.php`, lalu membuat commit merge
`merge: selesaikan conflict navbar`.

## Riwayat Praktikum Git
PS C:\xampp\htdocs\telkom-company-profile> git log --oneline --graph --decorate --all
*   0009409 (HEAD -> main, origin/main, origin/HEAD) docs: commit hasil perubahan yang terjadi di laptop b
|\
| * d6e4070 Simulasi: menambahkan isi baru Readme
* | d0f7094 simulasi docs: tambah catatan dari Laptop A
|/
* 85b4d07 docs:perbarui README dari laptop B
*   25bad25 merge: selesaikan conflict navbar
|\
| * 5e1165e (conflict-navbar) feat: ubah label profil pada branch conflict
* | 408844d style: ubah label profil pada main
|/
* 3056f5f feat: tambahkan informasi fokus pembelajaran
* f2f6a42 feat: tambahkan form admin lokal untuk berita
* 0e094dd feat: simpan pesan kontak ke database
* 4bda331 feat: tambahkan daftar dan detail berita
* 93d96f7 feat: hubungkan database dan tampilkan program studi
* 002db57 feat: tambahkan layout dasar dan stylesheet
* 5e76580 chore: inisialisasi project dan dokumentasi awal    

## Catatan
Seluruh konten institusi bersifat simulasi untuk pembelajaran.