### Seksi 2. Python Refresher

#### Video 4. Pemformatan String di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Pemformatan String dengan F-String:**

   - F-String adalah fitur baru yang diperkenalkan di Python 3.6, memungkinkan kita untuk memasukkan variabel langsung ke dalam string.
   - F-String dimulai dengan huruf `f` sebelum tanda kutip.

   **Contoh Kode:**

   ```python
   name = "Bob"
   greeting = f"Hello, {name}"
   print(greeting)  # Output: Hello, Bob
   ```

   - Jika variabel `name` diubah, string yang telah dibuat dengan F-String tidak berubah.

   **Contoh Kode:**

   ```python
   name = "Rolf"
   print(greeting)  # Output: Hello, Bob
   ```

2. **Penggunaan Dinamis dengan F-String:**

   - Jika ingin menggunakan nilai terbaru dari variabel, bisa langsung menggunakan F-String dalam `print`.

   **Contoh Kode:**

   ```python
   name = "Rolf"
   print(f"Hello, {name}")  # Output: Hello, Rolf
   ```

3. **Pemformatan String dengan `format()`:**

   - Metode lain untuk pemformatan string adalah dengan menggunakan `format()`.
   - Ini memungkinkan kita membuat template string yang dapat digunakan kembali dengan mengganti placeholder `{}` dengan nilai yang diinginkan.

   **Contoh Kode:**

   ```python
   greeting = "Hello, {}"
   with_name = greeting.format("Bob")
   print(with_name)  # Output: Hello, Bob
   ```

   - Template ini bisa digunakan kembali dengan nilai yang berbeda.

   **Contoh Kode:**

   ```python
   with_name = greeting.format("Rolf")
   print(with_name)  # Output: Hello, Rolf
   ```

4. **Pemanfaatan `format()` untuk String yang Lebih Panjang:**

   - `format()` juga dapat digunakan untuk string yang lebih panjang dengan beberapa placeholder.

   **Contoh Kode:**

   ```python
   longer_phrase = "Hello, {}. Today is {}."
   result = longer_phrase.format("Rolf", "Monday")
   print(result)  # Output: Hello, Rolf. Today is Monday.
   ```

5. **Kesimpulan:**
   - F-String adalah cara utama untuk melakukan pemformatan string di Python 3.6 ke atas, tetapi `format()` bisa berguna untuk membuat template yang dapat digunakan kembali.
   - Ada metode lama untuk pemformatan string yang tidak dibahas dalam video ini karena jarang digunakan.

---

Rangkuman ini menyoroti dua metode utama untuk pemformatan string di Python: F-String dan `format()`. Disertakan pula contoh kode untuk setiap metode, memudahkan pemahaman tentang bagaimana variabel dapat disisipkan ke dalam string dengan cara yang berbeda.
