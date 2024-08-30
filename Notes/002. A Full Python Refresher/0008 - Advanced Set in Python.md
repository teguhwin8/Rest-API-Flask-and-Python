### Seksi 2. Python Refresher

#### Video 8. Operasi Lanjutan pada Set

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Mendefinisikan Set:**

   - Set adalah kumpulan elemen unik yang didefinisikan dengan menggunakan tanda kurung kurawal `{}`. Jika set hanya memiliki satu elemen, cukup tuliskan elemen tersebut tanpa koma.

   **Contoh Kode:**

   ```python
   friends = {"Bob", "Rolf", "Anne"}
   abroad = {"Bob", "Anne"}
   ```

2. **Operasi `difference`:**

   - `difference` digunakan untuk menghitung selisih antara dua set. Operasi ini menghapus elemen yang ada di set lain dari set pertama.

   **Contoh Kode:**

   ```python
   local_friends = friends.difference(abroad)
   print(local_friends)  # Output: {"Rolf"}
   ```

   - Jika menggunakan `difference` dengan urutan terbalik, hasilnya akan berbeda.

   **Contoh Kode:**

   ```python
   abroad_difference = abroad.difference(friends)
   print(abroad_difference)  # Output: set()
   ```

3. **Operasi `union`:**

   - `union` digunakan untuk menggabungkan dua set, menghasilkan set baru yang berisi semua elemen dari kedua set tanpa duplikat.

   **Contoh Kode:**

   ```python
   friends = local_friends.union(abroad)
   print(friends)  # Output: {"Bob", "Rolf", "Anne"}
   ```

4. **Operasi `intersection`:**

   - `intersection` digunakan untuk menemukan elemen yang ada di kedua set. Ini akan memberikan elemen yang ada di kedua set tersebut.

   **Contoh Kode:**

   ```python
   art_friends = {"Bob", "Jen", "Rolf", "Charlie"}
   science_friends = {"Bob", "Jen", "Adam", "Anne"}
   both = art_friends.intersection(science_friends)
   print(both)  # Output: {"Bob", "Jen"}
   ```

5. **Set Kosong:**

   - Set kosong bisa didefinisikan dengan menggunakan `set()`.

   **Contoh Kode:**

   ```python
   empty_set = set()
   print(empty_set)  # Output: set()
   ```

6. **Penerapan dan Latihan:**

   - Penggunaan operasi set seperti `difference`, `union`, dan `intersection` sangat berguna dalam situasi di mana kita perlu mengelola dan membandingkan data unik. Mencoba berbagai kombinasi operasi ini akan membantu memperdalam pemahaman tentang bagaimana set berfungsi di Python.

7. **Sumber Daya Tambahan:**
   - Untuk memperdalam pemahaman tentang operasi set, berikut beberapa sumber daya yang bisa kamu eksplorasi:
     - [Python Set Operators](https://blog.teclado.com/python-set-operators/)
     - [Python Symmetric Difference](https://blog.teclado.com/python-symmetric-difference/)
     - [30 Days of Python: Day 11 - Sets](https://teclado.com/30-days-of-python/python-30-day-11-sets/)

---

Rangkuman ini mencakup operasi lanjutan pada set di Python, termasuk `difference`, `union`, dan `intersection`. Disertakan juga contoh kode untuk setiap operasi, membantu dalam memahami penerapannya secara praktis. Sumber daya tambahan disediakan untuk eksplorasi lebih lanjut.
