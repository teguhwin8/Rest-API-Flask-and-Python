### Seksi 2. Python Refresher
#### Video 13. If Statements dengan Kata Kunci `in` dan Contoh Lainnya

---

**Rangkuman:**

**Poin-Poin Penting:**

1. **If Statements dengan Kata Kunci `in`:**
   - Anda bisa menggunakan kata kunci `in` dalam if statement untuk memeriksa apakah suatu elemen ada dalam list, tuple, set, atau string, dan kemudian melakukan tindakan berdasarkan hasil pemeriksaan tersebut.

   **Contoh Kode:**
   ```python
   movies_watched = {"The Matrix", "Inception", "Interstellar"}
   user_movie = input("Enter a movie you've watched recently: ")

   if user_movie in movies_watched:
       print(f"I've watched {user_movie} too!")
   else:
       print("I haven't watched that yet.")
   ```

2. **Contoh Aplikasi: Magic Number:**
   - Sebuah contoh aplikasi sederhana yang meminta pengguna untuk menebak sebuah angka "ajaib". Program ini memeriksa apakah tebakan pengguna benar, memberikan petunjuk jika salah, dan memberikan pesan berdasarkan hasil tebakan.

   **Contoh Kode:**
   ```python
   number = 7
   user_input = input("Enter 'Y' if you would like to play: ")

   if user_input.lower() == 'y':
       user_number = int(input("Guess our number: "))

       if user_number == number:
           print("You guessed correctly!")
       elif abs(number - user_number) == 1:
           print("You were off by one.")
       else:
           print("Sorry, it's wrong.")
   ```

3. **Penggunaan Kata Kunci `in` untuk Berbagai Opsi Input:**
   - Anda bisa menggunakan `in` untuk menerima beberapa opsi input dari pengguna, seperti 'Y' atau 'y', dengan menggunakan tuple atau list.

   **Contoh Kode:**
   ```python
   if user_input in ('Y', 'y'):
       # Lanjutkan permainan
   ```

4. **Memberikan Petunjuk dengan `in`:**
   - Dengan kata kunci `in`, Anda bisa memberikan petunjuk jika tebakan pengguna mendekati angka "ajaib".

   **Contoh Kode:**
   ```python
   elif (number - user_number) in (1, -1):
       print("You were off by one.")
   ```

5. **Penggunaan `abs()` untuk Perbandingan:**
   - `abs()` digunakan untuk mendapatkan nilai absolut, yang memudahkan perbandingan dalam situasi seperti memeriksa seberapa dekat tebakan pengguna dengan angka yang benar.

   **Contoh Kode:**
   ```python
   elif abs(number - user_number) == 1:
       print("You were off by one.")
   ```

---

**Kesimpulan:**
- Video ini memberikan contoh-contoh bagaimana menggunakan kata kunci `in` dalam if statements untuk memeriksa keanggotaan elemen dalam struktur data seperti set dan tuple. Selain itu, contoh aplikasi "Magic Number" membantu memperjelas penggunaan logika if statement dan menunjukkan cara memberikan umpan balik kepada pengguna berdasarkan input mereka. Konsep-konsep ini sangat penting untuk membuat program interaktif yang responsif terhadap input pengguna.