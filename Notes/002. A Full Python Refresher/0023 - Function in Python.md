### Seksi 2. Python Refresher

#### Video 23. Fungsi di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Membuat Fungsi di Python:**

   - Untuk membuat fungsi di Python, gunakan kata kunci `def` diikuti dengan nama fungsi, tanda kurung, dan titik dua.
   - Fungsi berisi blok kode yang dapat dipanggil kapan saja menggunakan nama fungsinya.

   **Contoh Kode:**

   ```python
   def halo():
       print("Halo Dunia!")

   # Memanggil fungsi
   halo()
   ```

2. **Menjalankan Fungsi:**
   - Definisi fungsi tidak akan menjalankan fungsinya. Fungsi hanya berjalan jika dipanggil dengan menuliskan nama fungsinya diikuti dengan tanda kurung.
3. **Fungsi dengan Input Pengguna:**

   - Fungsi dapat digunakan untuk mengambil input dari pengguna dan mengelola logika pemrosesan data tersebut.

   **Contoh Kode:**

   ```python
   def umur_dalam_detik():
       umur = int(input("Masukkan umur Anda: "))
       umur_detik = umur * 365 * 24 * 60 * 60
       print(f"Umur Anda dalam detik adalah {umur_detik} detik.")

   umur_dalam_detik()
   ```

4. **Menghindari Kesalahan dalam Pembuatan Fungsi:**

   - **Menghindari Shadowing:** Jangan menggunakan nama variabel yang sama di dalam dan di luar fungsi, karena Python akan membuat ruang variabel terpisah dalam fungsi.

   **Contoh Kode yang Salah:**

   ```python
   teman = []

   def tambah_teman(nama_teman):
       teman = teman + [nama_teman]  # Kesalahan, menggunakan variabel yang belum didefinisikan di dalam fungsi
   ```

   **Contoh yang Benar:**

   ```python
   teman = []

   def tambah_teman(nama_teman):
       teman.append(nama_teman)  # Menggunakan method yang tidak mendefinisikan ulang variabel teman
   ```

5. **Urutan Definisi dan Pemanggilan Fungsi:**

   - Fungsi harus didefinisikan terlebih dahulu sebelum dipanggil dalam kode. Jika tidak, Python akan menghasilkan error bahwa fungsi belum terdefinisi.

6. **Penerapan di Kehidupan Nyata:**

   - **Aplikasi Restoran:**
     Fungsi dapat digunakan untuk mengelola pesanan pelanggan dan menghitung total harga.

   **Contoh Kode:**

   ```python
   def hitung_total(harga, jumlah):
       return harga * jumlah

   def tampilkan_pesanan(nama_pelanggan, nama_menu, harga, jumlah):
       total = hitung_total(harga, jumlah)
       print(f"Pesanan {nama_pelanggan}: {jumlah} {nama_menu} dengan total harga Rp{total}")

   # Contoh penggunaan
   tampilkan_pesanan("Ani", "Nasi Goreng", 20000, 2)
   ```

7. **Penerapan dalam Manajemen Data Siswa:**

   - Fungsi bisa digunakan untuk mengelola data siswa seperti menambahkan siswa baru atau menghitung nilai rata-rata kelas.

   **Contoh Kode:**

   ```python
   siswa = []

   def tambah_siswa(nama, nilai):
       siswa.append({"nama": nama, "nilai": nilai})

   def hitung_rata_rata():
       total_nilai = sum([s["nilai"] for s in siswa])
       return total_nilai / len(siswa)

   # Contoh penggunaan
   tambah_siswa("Budi", 85)
   tambah_siswa("Dewi", 90)
   print(f"Rata-rata nilai kelas: {hitung_rata_rata()}")
   ```

Dengan memahami fungsi, kita bisa membagi program menjadi bagian-bagian yang lebih mudah dikelola dan dipanggil kembali sesuai kebutuhan.
