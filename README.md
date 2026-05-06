# Laporan Praktikum Git & GitHub

**Nama:** Andhika Farhan Saputra  
**NIM:** 25/565469/SV/26953  
**Kelas:** A2
**Repository:** `praktikum-git-565469`


---

## Deskripsi Project
Project ini merupakan implementasi halaman web sederhana (seperti Toko Bunga Online) yang dibangun untuk memenuhi tugas praktikum alur kerja Git dan GitHub. Tujuan utama repositori ini adalah sebagai dokumentasi praktik manajemen versi (version control), yang mencakup proses inisialisasi, *branching*, pembuatan *Pull Request*, resolusi *merge conflict*, dan pelacakan masalah (*Issue Tracking*).

---

## TUGAS 1: Inisialisasi & Commit History

Pada tahap ini, repositori baru berhasil dibuat dan dihubungkan ke komputer lokal.

1. **Pembuatan Repository GitHub:** Repository dibuat dengan status Public dengan nama `praktikum-git-565469`.
   ![Create Repository](Create%20New%20Repository.jpeg)

2. **Cloning ke Lokal:** Repository di-clone ke dalam direktori lokal menggunakan terminal VS Code melalui perintah `git clone`.
   ![Cloning Repo](Comment%20Cloning%20Repository%20ke%20VSCode%20.jpeg)

---

## TUGAS 2: Branching & Pull Request

Pengembangan proyek dipisah dari branch utama (`main`) untuk mencegah perubahan tak terduga.

1. **Pembuatan Branch Baru:** Branch fitur baru dibuat secara lokal dari branch `main`.
   ![Create Branch](Create%20New%20Branch%20.jpeg)

2. **Membuat Pull Request (PR):** Setelah branch di-push, dilakukan pengajuan *Pull Request* (contoh pada branch `feature/navbar`).
   ![Compare PR](Compare%20and%20New%20Request%20.jpeg)

3. **Proses Merging:** Penggabungan *Pull Request* dilakukan setelah tidak ada masalah. Contoh di bawah ini adalah proses *Confirm merge* untuk branch `hotfix/typo` ke dalam branch `main`.
   ![Confirm Merge](Confirm%20Merge%20.jpeg)

---

## TUGAS 3: Konflik & Rebase

Simulasi bentrok antar kode (conflict) berhasil dilakukan dengan mengubah baris CSS (warna background) yang sama pada dua branch *experiment*.

1. **Penyelesaian Konflik di VS Code:** Terjadi konflik antara branch `experiment/color-b` (Current Change) dan `main` (Incoming Change). Resolusi dilakukan secara manual melalui antarmuka editor.
   ![Simulasi Konflik](Simulasi%20Conflict%20.jpeg)

2. **Konfirmasi Penggabungan Setelah Konflik:** Setelah konflik CSS tersebut di-resolve, proses *merge* dapat dilanjutkan kembali tanpa *blocking*.
   ![Simulasi After Conflict](Simulasi%20After%20Conflict.jpeg)

---

## TUGAS 4: Dokumentasi & Issue Tracking

Manajemen bug dan penambahan fitur dicatat dengan rapi menggunakan GitHub Issues agar terhubung dengan status *Pull Request*.

1. **Membuat Issue:** Melaporkan *Issue* baru terkait deskripsi gambar dan item yang tidak cocok.
   ![Create Issue](Create%20New%20Issue%20.jpeg)

2. **Menutup Issue Otomatis via PR:** Issue yang telah dibuat (Issue #8) ditautkan dan ditutup secara otomatis menggunakan kata kunci `Closes #8` di dalam deskripsi *Pull Request*.
   ![Closes Issue](Closes%20Image%20Issue.jpeg)

---

## Dokumentasi Perintah Git yang Digunakan

Berikut adalah perintah Git yang dipraktikkan selama pengerjaan proyek ini:

| Perintah | Penjelasan Singkat |
| :--- | :--- |
| `git clone [url]` | Menggandakan repositori dari GitHub ke penyimpanan komputer lokal. |
| `git add .` | Menambahkan semua file yang berubah ke *staging area* sebelum disimpan. |
| `git commit -m "[pesan]"` | Menyimpan riwayat perubahan ke repositori lokal beserta pesan konvensinya. |
| `git push` | Mengunggah riwayat commit dan branch dari lokal ke GitHub (remote). |
| `git checkout -b [branch]` / `switch` | Membuat dan langsung berpindah ke cabang (*branch*) baru. |
| `git merge [branch]` | Menggabungkan riwayat dari branch lain ke branch yang saat ini aktif. |
| `git log --oneline --graph` | Menampilkan ringkasan riwayat dan visualisasi garis percabangan commit. |
| `git rebase -i` | Memanipulasi atau menggabungkan (*squash*) beberapa commit menjadi satu kesatuan. |