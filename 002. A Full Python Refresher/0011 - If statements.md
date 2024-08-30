### Seksi 2. Python Refresher

#### Video 11. Memahami If Statements di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Penggunaan If Statements:**

   - If statement memungkinkan kita membuat keputusan berdasarkan nilai Boolean dalam program. If statements digunakan untuk menjalankan blok kode tertentu jika kondisi yang diberikan adalah `True`.

   **Contoh Kode:**

   ```python
   day_of_week = input("What day of the week is it today? ")

   if day_of_week == "Monday":
       print("Have a great start to your week!")
   ```

2. **Indentasi dalam If Statements:**

   - Python menggunakan indentasi untuk menentukan blok kode yang akan dijalankan di dalam if statement. Biasanya, indentasi menggunakan 4 spasi untuk konsistensi.

   **Contoh Kode:**

   ```python
   if day_of_week == "Monday":
       print("Have a great start to your week!")
   print("This always runs.")  # Kode ini akan selalu dijalankan
   ```

3. **Penggunaan Else dan Elif:**

   - `else` digunakan untuk menentukan blok kode yang akan dijalankan jika kondisi `if` adalah `False`.
   - `elif` (else if) digunakan untuk memeriksa kondisi tambahan jika kondisi `if` pertama adalah `False`.

   **Contoh Kode:**

   ```python
   if day_of_week == "Monday":
       print("Have a great start to your week!")
   elif day_of_week == "Tuesday":
       print("Full speed ahead!")
   else:
       print("Have a nice day!")
   ```

4. **Menghindari Duplikasi Perbandingan:**

   - Jika Anda menggunakan `if` dan `else`, Python hanya akan memeriksa satu kondisi. Ini lebih efisien dibandingkan memeriksa beberapa kondisi secara terpisah.

5. **Mengatasi Masalah Input Pengguna:**

   - Pengguna mungkin tidak memasukkan input dengan format yang Anda harapkan, seperti memasukkan huruf kecil ketika huruf besar diharapkan. Untuk mengatasi ini, Anda dapat mengonversi input pengguna ke huruf kecil menggunakan `.lower()`.

   **Contoh Kode:**

   ```python
   day_of_week = input("What day of the week is it today? ").lower()

   if day_of_week == "monday":
       print("Have a great start to your week!")
   elif day_of_week == "tuesday":
       print("Full speed ahead!")
   else:
       print("Have a nice day!")
   ```

6. **Manfaat Konversi Huruf Kecil:**
   - Dengan mengonversi input dan perbandingan ke huruf kecil, program Anda akan lebih fleksibel dalam menangani variasi input pengguna, seperti "Monday", "monday", atau "MONDAY".

---

**Kesimpulan:**

- If statements adalah alat penting dalam pemrograman Python yang memungkinkan pengambilan keputusan berdasarkan kondisi tertentu. Penggunaan `else` dan `elif` membantu menyederhanakan logika dalam program. Selain itu, mengelola input pengguna dengan metode seperti `.lower()` dapat membuat program Anda lebih tahan terhadap variasi input.
