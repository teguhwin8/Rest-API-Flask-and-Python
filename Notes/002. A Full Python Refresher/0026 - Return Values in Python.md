### Seksi 2. Python Refresher

#### Video 26. Return Values in Python

---

**Poin-Poin Penting:**

1. **Nilai Kembali (Return Values) dalam Fungsi:**

   - Fungsi di Python secara default **mengembalikan** `None` jika tidak ada pernyataan `return`.
   - Untuk mengembalikan hasil perhitungan atau nilai lain, gunakan kata kunci `return` di dalam fungsi.

   **Contoh Kode:**

   ```python
   def tambah(x, y):
       return x + y

   hasil = tambah(5, 8)
   print(hasil)  # Akan mencetak 13
   ```

2. **Fungsi Mengembalikan `None` Secara Default:**

   - Jika fungsi tidak mengandung `return`, fungsi tersebut akan mengembalikan `None`.

   **Contoh Kode yang Mengembalikan `None`:**

   ```python
   def tanpa_return(x, y):
       print(x + y)

   hasil = tanpa_return(5, 8)
   print(hasil)  # Akan mencetak None karena tidak ada return
   ```

3. **Perbedaan Antara `print` dan `return`:**

   - `print` hanya menampilkan nilai ke layar tetapi tidak mengembalikannya ke pemanggil fungsi. `return` mengembalikan nilai sehingga bisa digunakan dalam perhitungan atau logika selanjutnya.

   **Contoh:**

   ```python
   def tambah(x, y):
       print(x + y)  # Mencetak hasil tetapi tidak mengembalikan

   hasil = tambah(5, 8)  # hasil akan None karena fungsi tidak mengembalikan apapun
   print(hasil)  # Akan mencetak None
   ```

4. **Menggunakan `return` untuk Menghentikan Fungsi:**

   - Ketika `return` dijalankan, fungsi langsung berhenti, dan kode setelah `return` tidak akan dieksekusi.

   **Contoh Kode:**

   ```python
   def contoh_fungsi():
       return "Ini dikembalikan"
       print("Ini tidak akan pernah dicetak")  # Baris ini tidak akan dijalankan

   hasil = contoh_fungsi()
   print(hasil)  # Akan mencetak "Ini dikembalikan"
   ```

5. **Mengembalikan Nilai yang Berbeda Berdasarkan Kondisi:**

   - Anda dapat mengembalikan berbagai nilai berdasarkan kondisi dalam fungsi, tetapi disarankan untuk mengembalikan nilai dengan tipe data yang konsisten.

   **Contoh Kode:**

   ```python
   def bagi(dividen, pembagi):
       if pembagi == 0:
           return "Tidak bisa membagi dengan nol"
       return dividen / pembagi

   hasil = bagi(10, 2)
   print(hasil)  # Akan mencetak 5.0
   ```

6. **Penerapan di Kehidupan Nyata:**

   **Contoh Aplikasi di Sistem Bank:**

   - Dalam aplikasi perbankan, kita bisa menggunakan fungsi untuk menghitung bunga berdasarkan kondisi tertentu.

   **Contoh Kode:**

   ```python
   def hitung_bunga(saldo, bunga_persen):
       if saldo < 0:
           return "Saldo negatif tidak dapat dihitung bunganya"
       return saldo * bunga_persen / 100

   hasil_bunga = hitung_bunga(1000000, 5)  # Menghitung bunga 5% dari saldo Rp1.000.000
   print(f"Bunga yang diterima: Rp{hasil_bunga}")
   ```

   **Contoh Aplikasi di Restoran:**

   - Dalam aplikasi kasir restoran, kita bisa menghitung total tagihan dengan menambahkan pajak dan diskon.

   **Contoh Kode:**

   ```python
   def hitung_total(harga, pajak=10, diskon=0):
       total = harga + (harga * pajak / 100) - (harga * diskon / 100)
       return total

   total_tagihan = hitung_total(50000, diskon=5)  # Menghitung total dengan diskon 5%
   print(f"Total yang harus dibayar: Rp{total_tagihan}")
   ```

---

Dengan menggunakan `return` dalam fungsi, kita bisa membuat kode lebih dinamis dan memungkinkan hasil dari fungsi digunakan dalam perhitungan atau logika lain. Ini adalah konsep penting untuk membangun program yang lebih modular dan fleksibel.
