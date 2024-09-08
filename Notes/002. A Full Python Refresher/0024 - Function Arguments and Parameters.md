### Seksi 2. Python Refresher

#### Video 24. Function Arguments dan Parameters di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Pengertian Parameter dan Argumen:**

   - **Parameter** adalah variabel yang didefinisikan di dalam tanda kurung saat membuat fungsi.
   - **Argumen** adalah nilai yang diberikan kepada parameter saat fungsi dipanggil.

   **Contoh Kode:**

   ```python
   def tambah(x, y):  # x dan y adalah parameter
       hasil = x + y
       print(hasil)

   tambah(5, 3)  # 5 dan 3 adalah argumen
   ```

2. **Fungsi dengan Argumen dan Tanpa Argumen:**

   - Fungsi bisa memiliki parameter atau tidak, dan jika ada parameter, maka saat fungsi dipanggil harus memberikan nilai untuk parameter tersebut.

   **Contoh Kode Tanpa Argumen:**

   ```python
   def halo():
       print("Halo Dunia!")

   halo()  # Fungsi dipanggil tanpa argumen
   ```

   **Contoh Kode Dengan Argumen:**

   ```python
   def sapa(nama):
       print(f"Halo {nama}!")

   sapa("Ani")  # Argumen diberikan
   ```

3. **Positional Argument (Argumen Berdasarkan Posisi):**

   - Posisi argumen menentukan nilai dari parameter dalam fungsi.

   **Contoh Kode:**

   ```python
   def nama_lengkap(depan, belakang):
       print(f"Nama lengkap: {depan} {belakang}")

   nama_lengkap("Budi", "Santoso")  # "Budi" untuk 'depan', "Santoso" untuk 'belakang'
   ```

4. **Keyword Argument (Argumen Berdasarkan Nama):**

   - Selain berdasarkan posisi, kita juga bisa memberikan argumen berdasarkan nama parameternya, ini membuat kode lebih jelas.

   **Contoh Kode:**

   ```python
   def nama_lengkap(depan, belakang):
       print(f"Nama lengkap: {depan} {belakang}")

   nama_lengkap(depan="Budi", belakang="Santoso")
   nama_lengkap(belakang="Santoso", depan="Budi")  # Urutannya bisa diubah karena menggunakan keyword
   ```

5. **Menggabungkan Positional dan Keyword Arguments:**

   - Argumen berbasis posisi harus ditempatkan sebelum argumen berbasis keyword.

   **Contoh Kode:**

   ```python
   def bagi(angka1, angka2):
       if angka2 == 0:
           print("Pembagian dengan nol tidak diperbolehkan!")
       else:
           print(angka1 / angka2)

   bagi(10, angka2=2)  # Kombinasi positional dan keyword argument
   ```

6. **Penerapan di Kehidupan Nyata:**

   - **Contoh Aplikasi Pembelian Makanan:**
     Dalam aplikasi restoran, kita bisa membuat fungsi untuk menghitung total harga makanan berdasarkan nama makanan, harga, dan jumlah yang dipesan.

   **Contoh Kode:**

   ```python
   def hitung_total(nama_makanan, harga_satuan, jumlah):
       total_harga = harga_satuan * jumlah
       print(f"Pesanan: {nama_makanan}, Jumlah: {jumlah}, Total: Rp{total_harga}")

   # Contoh penggunaan
   hitung_total("Nasi Goreng", 20000, 2)
   ```

   - **Contoh Aplikasi Sekolah:**
     Untuk menghitung nilai rata-rata siswa dalam suatu mata pelajaran.

   **Contoh Kode:**

   ```python
   def hitung_rata_rata(nama_siswa, nilai_uts, nilai_uas):
       rata_rata = (nilai_uts + nilai_uas) / 2
       print(f"Nama: {nama_siswa}, Nilai Rata-Rata: {rata_rata}")

   # Contoh penggunaan
   hitung_rata_rata("Ani", 85, 90)
   ```

Penggunaan keyword arguments akan sangat membantu dalam meningkatkan keterbacaan kode dan membuatnya lebih jelas, terutama dalam situasi yang melibatkan banyak parameter atau argumen yang kompleks.
