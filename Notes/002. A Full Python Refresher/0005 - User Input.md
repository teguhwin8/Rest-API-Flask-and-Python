### Seksi 2. Python Refresher

#### Video 5. Mendapatkan Input dari Pengguna

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Mendapatkan Input dari Pengguna:**

   - Untuk mendapatkan input dari pengguna, kita bisa menggunakan fungsi `input()`, yang akan menampilkan prompt dan menunggu pengguna memasukkan data.
   - Input yang diperoleh selalu dalam bentuk string.

   **Contoh Kode:**

   ```python
   name = input("Enter your name: ")
   print(name)  # Output: Rolf (misalnya jika pengguna memasukkan Rolf)
   ```

2. **Mengubah Input Menjadi Angka:**

   - Jika ingin melakukan operasi matematika pada input, kita harus mengonversinya dari string ke tipe data numerik seperti integer (`int`) atau float (`float`).

   **Contoh Kode:**

   ```python
   size_input = input("Enter the size in square feet: ")
   square_feet = int(size_input)  # Konversi dari string ke integer
   square_metres = square_feet / 10.8
   print(f"{square_feet} square feet is {square_metres} square metres")
   ```

3. **Penanganan Error Tipe:**

   - Jika mencoba melakukan operasi matematika pada string tanpa konversi, Python akan mengembalikan error tipe karena tidak bisa mengoperasikan string dan angka.

   **Contoh Error:**

   ```python
   size_input = input("Enter the size in square feet: ")
   square_metres = size_input / 10.8  # Ini akan mengakibatkan TypeError
   ```

4. **Pemformatan Output dengan F-String:**

   - Dengan menggunakan F-String, kita bisa membuat output yang lebih baik, misalnya untuk mencetak hasil perhitungan dengan format yang lebih rapi.

   **Contoh Kode:**

   ```python
   print(f"{square_feet} square feet is {square_metres:.2f} square metres")
   ```

   - Sintaks `:.2f` pada F-String digunakan untuk membatasi jumlah angka desimal menjadi dua digit.

5. **Pemanfaatan Fungsi `int()` dan `float()`:**

   - Fungsi `int()` mengonversi string menjadi integer (bilangan bulat).
   - Fungsi `float()` mengonversi string menjadi bilangan desimal.

   **Contoh Kode:**

   ```python
   square_feet = int(input("Enter the size in square feet: "))
   square_metres = square_feet / 10.8
   print(f"{square_feet} square feet is {square_metres:.2f} square metres")
   ```

6. **Kesimpulan:**
   - Video ini mengajarkan cara mendapatkan input dari pengguna dan mengonversinya ke tipe data numerik untuk keperluan perhitungan, serta cara memformat output menggunakan F-String untuk menampilkan hasil dengan lebih baik.

---

Rangkuman ini mencakup bagaimana mendapatkan input dari pengguna, mengonversi input menjadi angka, dan menampilkan hasil perhitungan dengan format yang rapi menggunakan F-String. Contoh kode disertakan untuk memperjelas setiap konsep yang dibahas.
