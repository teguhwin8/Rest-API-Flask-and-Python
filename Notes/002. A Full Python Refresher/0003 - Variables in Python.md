### Seksi 2. Python Refresher

#### Video 3. Variabel dalam Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Definisi Variabel:**

   - Sebuah variabel di Python adalah nama untuk sebuah nilai. Ini mirip dengan variabel dalam aljabar, namun dengan beberapa perbedaan yang akan lebih jelas seiring kamu belajar Python.

2. **Cara Menetapkan Variabel:**

   - Variabel ditetapkan dengan menuliskan nama variabel, diikuti oleh tanda sama dengan `=`, dan kemudian nilai yang ingin diberikan, misalnya `x = 15`.

   **Contoh Kode:**

   ```python
   x = 15
   ```

3. **Operasi pada Variabel:**

   - Python terlebih dahulu membuat nilai di sebelah kanan tanda sama dengan sebelum menetapkan nama variabel.

   **Contoh Kode:**

   ```python
   price = 9.99
   discount = 0.2
   result = price * (1 - discount)
   print(result)  # Output: 7.992
   ```

4. **Tipe Data Lainnya:**

   - **String:** Tipe data untuk menyimpan karakter, seperti nama atau nomor telepon.

   **Contoh Kode:**

   ```python
   name = "Rolf"
   print(name)  # Output: Rolf
   ```

   - String dapat diisi ulang dengan nilai baru:

   **Contoh Kode:**

   ```python
   name = "Bob"
   print(name)  # Output: Bob
   ```

5. **Penggunaan String:**

   - Operasi pada string seperti `name * 2` akan menghasilkan pengulangan string tersebut.

   **Contoh Kode:**

   ```python
   name = "Rolf"
   print(name * 2)  # Output: RolfRolf
   ```

6. **Penetapan Variabel dengan Nilai yang Sama:**

   - Misalnya `a = 25` dan `b = a` akan menjadikan `b` juga bernilai `25`.

   **Contoh Kode:**

   ```python
   a = 25
   b = a
   print(a, b)  # Output: 25 25
   ```

   - Jika `b` kemudian diberi nilai baru, maka hanya `b` yang berubah, `a` tetap bernilai `25`.

   **Contoh Kode:**

   ```python
   b = 17
   print(a, b)  # Output: 25 17
   ```

7. **Kesimpulan:**
   - Video ini memberikan penyegaran tentang konsep variabel di Python. Tidak semua detail akan dijelaskan di sini, karena ini bukan kursus pengantar Python, melainkan untuk mengingatkan kembali dasar-dasar bagi yang sudah berpengalaman.

---

Rangkuman ini menyoroti poin-poin penting tentang bagaimana variabel bekerja di Python, termasuk cara menetapkan, menggunakan, dan mengubahnya, serta memberikan contoh kode yang relevan untuk memudahkan pemahaman.
