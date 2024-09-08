### Seksi 2. Python Refresher

#### Video 25. Default Parameter Values di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Default Parameter (Parameter Bawaan):**

   - Dalam Python, kita bisa memberikan nilai default untuk parameter pada fungsi. Jika argumen tidak diberikan saat pemanggilan fungsi, maka nilai default yang akan digunakan.

   **Contoh Kode:**

   ```python
   def tambah(x, y=8):  # y memiliki nilai default 8
       hasil = x + y
       print(hasil)

   tambah(5)  # Menggunakan nilai default y = 8
   tambah(5, 3)  # Menggantikan nilai default dengan argumen baru
   ```

2. **Posisi Parameter:**

   - Parameter dengan nilai default harus berada di akhir daftar parameter.
   - Parameter wajib (tanpa default) harus didefinisikan sebelum parameter dengan nilai default.

   **Contoh Kode yang Salah:**

   ```python
   def fungsi_salah(x=5, y):  # Ini akan menimbulkan error
       pass
   ```

   **Contoh Kode yang Benar:**

   ```python
   def fungsi_benar(x, y=5):
       pass
   ```

3. **Penggunaan Variabel sebagai Default:**

   - Nilai default parameter bisa berasal dari variabel, tapi penting diingat bahwa setelah fungsi didefinisikan, perubahan pada variabel tidak akan memengaruhi nilai default parameter.

   **Contoh Kode:**

   ```python
   default_y = 3

   def tambah(x, y=default_y):
       print(x + y)

   tambah(2)  # Akan menghasilkan 5, karena y = 3
   default_y = 10
   tambah(2)  # Masih akan menghasilkan 5, karena nilai default y sudah diatur sebelumnya
   ```

   - Oleh karena itu, lebih baik langsung memasukkan nilai default di dalam definisi fungsi.

4. **Penerapan di Kehidupan Nyata:**

   **Contoh Aplikasi di Restoran:**

   - Misalnya kita memiliki aplikasi restoran, di mana pesanan minuman memiliki harga default jika jenis minuman tidak disebutkan oleh pelanggan.

   **Contoh Kode:**

   ```python
   def hitung_harga_makanan(makanan, harga_makanan, harga_minuman=5000):
       total_harga = harga_makanan + harga_minuman
       print(f"Makanan: {makanan}, Total: Rp{total_harga}")

   # Contoh penggunaan
   hitung_harga_makanan("Nasi Goreng", 20000)  # Menggunakan harga minuman default Rp5000
   hitung_harga_makanan("Nasi Goreng", 20000, 10000)  # Harga minuman diganti dengan Rp10000
   ```

   **Contoh Aplikasi Sekolah:**

   - Dalam sistem penilaian siswa, kita bisa memberikan nilai default untuk tugas yang tidak dikerjakan.

   **Contoh Kode:**

   ```python
   def hitung_rata_rata(nilai_uts, nilai_uas, nilai_tugas=50):
       rata_rata = (nilai_uts + nilai_uas + nilai_tugas) / 3
       print(f"Nilai Rata-Rata: {rata_rata}")

   # Contoh penggunaan
   hitung_rata_rata(85, 90)  # Menggunakan nilai default tugas 50
   hitung_rata_rata(85, 90, 80)  # Nilai tugas diganti 80
   ```

---

Dengan penggunaan default parameter, kita bisa membuat fungsi lebih fleksibel dan lebih mudah digunakan, terutama ketika kita ingin nilai tertentu menjadi opsi bawaan jika tidak ada input yang diberikan.
