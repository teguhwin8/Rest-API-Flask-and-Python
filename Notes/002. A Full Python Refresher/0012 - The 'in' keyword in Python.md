### Seksi 2. Python Refresher
#### Video 12. Menggunakan Kata Kunci `in` di Python

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **Apa Itu Kata Kunci `in`:**
   - Kata kunci `in` digunakan di Python untuk memeriksa apakah suatu elemen ada di dalam list, tuple, set, atau string. Ini berguna untuk memeriksa keanggotaan elemen dalam struktur data.

2. **Penggunaan `in` pada List:**
   - Anda dapat menggunakan `in` untuk memeriksa apakah suatu elemen ada di dalam list.

   **Contoh Kode:**
   ```python
   friends = ["Rolf", "Bob", "Jen"]
   print("Jen" in friends)  # Output: True
   ```

3. **Penggunaan `in` pada Set:**
   - Set adalah struktur data yang unik, artinya tidak ada elemen yang duplikat. Kata kunci `in` juga dapat digunakan untuk memeriksa keanggotaan elemen dalam set.

   **Contoh Kode:**
   ```python
   movies_watched = {"The Matrix", "Inception", "Interstellar"}
   print("The Matrix" in movies_watched)  # Output: True
   print("Monty Python" in movies_watched)  # Output: False
   ```

4. **Penggunaan `in` pada String:**
   - `in` juga dapat digunakan untuk memeriksa apakah suatu substring ada di dalam string.

   **Contoh Kode:**
   ```python
   movie = "The Matrix"
   print("RIX" in movie)  # Output: True
   ```

5. **Keuntungan Menggunakan `in`:**
   - `in` sangat berguna untuk membuat keputusan cepat berdasarkan keanggotaan, misalnya dalam if statements, yang memungkinkan program Anda menjadi lebih dinamis dan responsif terhadap input pengguna.

---

**Kesimpulan:**
- Kata kunci `in` adalah alat yang sangat berguna di Python untuk memeriksa apakah suatu elemen ada di dalam list, tuple, set, atau string. Ini memungkinkan Anda untuk menulis kode yang lebih dinamis dan fleksibel. Dalam video selanjutnya, penggunaan `in` akan diperluas dengan if statements untuk menciptakan program yang lebih kompleks dan bermanfaat.