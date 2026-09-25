## LAPORAN DESAIN DAN PEMROGRAMAN WEB - JOBSHEET 4

#### **Nama**  : Rahma Aulia Nurrizky
#### **NIM**   : 254107020168
#### **Kelas** : TI-2A / 23

---

### Jobsheet 4 : Desain Layout, Wireframe, & RWD SIMPUS-Mini

---

### Wireframe & User Flow - SIMPUS-MINI
Sub-CPMK : Merancang UI/UX aplikasi (projek).

Halaman yg sudah ada (Beranda, Daftar Buku, Tambah Buku, Daftar Anggota, Tambah Anggota dari Jobsheet 1-3) belum mencakup fitur Login, Dashboard Petugas, Peminjaman dan Pengembalian. Dokumen ini merancang wireframe utk halaman-halaman tersebut sebelum diimplementasikan mulai Jobsheet 5 dan seterusnya.

### AKTOR
- **Tamu** : hanya bisa melihat katalog buku (Beranda, Daftar Buku) tanpa login.
- **Petugas** : melakukan login utk mengakses semua fitur CRUD dan transaksi peminjaman

### USER FLOW - Peminjaman Buku
```text
[Petugas Login] -> [Dashboard] -> [Pilih menu "Peminjaman Baru"]
                -> [Pilih Anggota] -> [Pilih Buku (stok > 0)]
                -> [Simpan] -> [Stok buku berkurang 1] -> [Kembali ke Dashboard]
```

#### USER FLOW - Pengembalian Buku
```text
[Dashboard] -> [Menu "Pengembalian"] -> [Cari transaksi aktif (anggota/buku)]
            -> [Tandai "Dikembalikan"] -> [Stok buku bertambah 1]
            -> [Kembali ke Dashboard]
```

### WIREFRAME - Halaman Login
```text
+-------------------------------------------------+
|                   SIMPUS-Mini                   |
|-------------------------------------------------|
|                                                 |
|                [ Login Petugas ]                |
|                                                 |
|       Username : [____________________]         |
|       Password : [____________________]         |
|                                                 |
|                   [  Masuk  ]                   |
|                                                 |
|         Belum punya akun? Daftar di sini        |
+-------------------------------------------------+
```

### WIREFRAME - Dashboard Petugas
```text
+---------------------------------------------------------------------------------+
| SIMPUS-Mini       Beranda | Buku | Anggota | Peminjaman | (Nama Petugas) Logout |
|---------------------------------------------------------------------------------|
|    [Total Buku]   [Total Anggota]   [Sedang Dipinjam]   [Buku Terlambat]        |
|                                                                                 |
|  Aksi Cepat:                                                                    |
|  [ + Peminjaman Baru ]   [ + Pengembalian ]                                     |
|                                                                                 |
|  Transaksi Terbaru                                                              |
|  ---------------------------------------------------------------------------    |
|  Anggota | Buku | Tanggal Pinjam | Status                                       |
+---------------------------------------------------------------------------------+
```

### WIREFRAME - Form Peminjaman
```text
+-------------------------------------------------+
| Form Peminjaman Buku                            |
|-------------------------------------------------|
| Anggota        : [ dropdown pilih anggota ]     |
| Buku           : [ dropdown, hanya stok > 0 ]   |
| Tanggal Pinjam : [ auto : hari ini ]            |
|                                                 |
|             [  Simpan Peminjaman  ]             |
+-------------------------------------------------+
```

### WIREFRAME - Form Pengembalian
```text
+-------------------------------------------------+
| Pengembalian Buku                               |
|-------------------------------------------------|
| Cari transaksi aktif :                          |
| [ nama anggota / judul buku _________________ ] |
|                                                 |
| Anggota | Buku | Tanggal Pinjam | [Kembalikan]  |
+-------------------------------------------------+
```

### WIREFRAME - Riwayat Peminjaman per Anggota
```text
+---------------------------------------------------+
| Riwayat Peminjaman - Siti Aminah                  |
|---------------------------------------------------|
| Buku            | Pinjam   | Kembali  | Status    |
| Laskar Pelangi  | 01/07    | 10/07    | Selesai   |
| Bumi Manusia    | 15/07    | -        | Dipinjam  |
+---------------------------------------------------+
```
