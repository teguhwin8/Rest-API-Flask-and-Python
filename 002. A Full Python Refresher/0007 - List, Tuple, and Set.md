### Seksi 2. Python Refresher

#### Video 7. Lists, Tuples, dan Sets di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Definisi Lists, Tuples, dan Sets:**

   - **Lists:** Kumpulan elemen yang didefinisikan menggunakan tanda kurung siku `[]`. Elemen-elemen dalam list bisa ditambahkan, dihapus, dan diubah.
   - **Tuples:** Mirip dengan list, tetapi didefinisikan menggunakan tanda kurung `()`. Elemen dalam tuple tidak bisa diubah, ditambahkan, atau dihapus setelah didefinisikan.
   - **Sets:** Kumpulan elemen yang didefinisikan menggunakan tanda kurung kurawal `{}`. Set tidak memperbolehkan elemen duplikat dan tidak menjamin urutan elemen.

   **Contoh Kode:**

   ```python
   l = ["Bob", "Rolf", "Anne"]  # List
   t = ("Bob", "Rolf", "Anne")  # Tuple
   s = {"Bob", "Rolf", "Anne"}  # Set
   ```

2. **Akses Elemen dalam List dan Tuple:**

   - Menggunakan notasi subscript `[index]` untuk mengakses elemen dalam list dan tuple. Indeks dimulai dari 0.

   **Contoh Kode:**

   ```python
   print(l[0])  # Output: Bob
   print(t[1])  # Output: Rolf
   ```

   - Set tidak mendukung akses elemen menggunakan indeks karena set tidak memiliki urutan yang tetap.

3. **Modifikasi List dan Tuple:**

   - **List:** Elemen dalam list bisa diubah menggunakan notasi subscript.

   **Contoh Kode:**

   ```python
   l[0] = "Smith"
   print(l)  # Output: ["Smith", "Rolf", "Anne"]
   ```

   - **Tuple:** Tidak bisa diubah setelah didefinisikan. Jika mencoba untuk mengubah elemen dalam tuple, Python akan menghasilkan error.

   **Contoh Error:**

   ```python
   t[0] = "Smith"  # Akan menghasilkan TypeError
   ```

4. **Menambahkan dan Menghapus Elemen:**

   - **List:** Elemen bisa ditambahkan menggunakan `append()` dan dihapus menggunakan `remove()`.

   **Contoh Kode:**

   ```python
   l.append("Smith")
   print(l)  # Output: ["Bob", "Rolf", "Anne", "Smith"]
   l.remove("Bob")
   print(l)  # Output: ["Rolf", "Anne", "Smith"]
   ```

   - **Set:** Elemen bisa ditambahkan menggunakan `add()` tetapi tidak bisa memiliki elemen duplikat. Elemen juga bisa dihapus.

   **Contoh Kode:**

   ```python
   s.add("Smith")
   print(s)  # Output: {"Anne", "Bob", "Smith", "Rolf"}
   s.add("Smith")
   print(s)  # Output: {"Anne", "Bob", "Smith", "Rolf"} (Smith hanya muncul sekali)
   ```

   - **Tuple:** Tidak bisa menambahkan atau menghapus elemen setelah didefinisikan.

5. **Kesimpulan:**
   - **Lists:** Fleksibel, memungkinkan penambahan, penghapusan, dan modifikasi elemen.
   - **Tuples:** Tidak bisa diubah setelah didefinisikan, cocok untuk data yang tidak perlu diubah.
   - **Sets:** Tidak memperbolehkan duplikat dan tidak menjamin urutan, cocok untuk data yang unik.

---

Rangkuman ini memberikan pengenalan tentang bagaimana menggunakan lists, tuples, dan sets di Python, termasuk cara mendefinisikan, mengakses, dan memodifikasi mereka. Disertakan contoh kode untuk memudahkan pemahaman setiap konsep yang dibahas.
