### Seksi 2. Python Refresher

#### Video 6. Membangun Aplikasi Pertama

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Tujuan Aplikasi:**

   - Aplikasi ini akan meminta pengguna untuk memasukkan usia mereka, dan kemudian menghitung berapa banyak bulan yang setara dengan usia tersebut.
   - Misalnya, jika pengguna memasukkan usia 10 tahun, aplikasi akan menghitung dan menampilkan 120 bulan (karena setiap tahun memiliki 12 bulan).

2. **Langkah-Langkah Pembangunan Aplikasi:**

   **a. Meminta Input Usia:**

   - Gunakan fungsi `input()` untuk meminta pengguna memasukkan usia mereka.
   - Karena `input()` selalu mengembalikan string, kita perlu mengonversi input menjadi integer menggunakan `int()`.

   **Contoh Kode:**

   ```python
   user_age = input("Enter your age: ")
   years = int(user_age)
   ```

   **b. Menghitung Jumlah Bulan:**

   - Setelah mendapatkan usia dalam tahun, kalikan dengan 12 untuk mendapatkan jumlah bulan.

   **Contoh Kode:**

   ```python
   months = years * 12
   ```

   **c. Mencetak Hasil:**

   - Gunakan F-String untuk menampilkan hasil dalam format yang mudah dibaca.

   **Contoh Kode:**

   ```python
   print(f"Your age, {years}, is equal to {months} months.")
   ```

3. **Optimisasi Kode:**

   - Untuk menyederhanakan kode, kita dapat langsung mengonversi input ke integer dalam satu langkah, tanpa perlu variabel sementara.

   **Contoh Kode yang Disederhanakan:**

   ```python
   years = int(input("Enter your age: "))
   months = years * 12
   print(f"Your age, {years}, is equal to {months} months.")
   ```

4. **Tantangan Tambahan:**

   - Sebagai latihan, cobalah memperluas aplikasi ini dengan menghitung dan mencetak jumlah detik yang setara dengan usia yang diberikan. Untuk melakukan ini, perlu memperhitungkan jumlah hari per tahun, jam per hari, menit per jam, dan detik per menit.

   **Petunjuk:**

   - Kamu perlu mengalikan usia dalam tahun dengan jumlah detik dalam satu tahun.

5. **Kesimpulan:**
   - Aplikasi sederhana ini adalah recap dari apa yang telah dipelajari, termasuk meminta input dari pengguna, mengonversi input, melakukan perhitungan, dan menampilkan hasil dengan format yang rapi.

---

Rangkuman ini menjelaskan langkah-langkah dalam membangun aplikasi pertama yang menghitung jumlah bulan berdasarkan usia pengguna, serta memberikan contoh kode untuk setiap langkah. Terdapat juga tantangan tambahan untuk menghitung jumlah detik, yang dapat membantu memperdalam pemahaman tentang konsep-konsep yang telah dipelajari.
