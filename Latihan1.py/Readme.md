
# 📌 **Penjelasan Program Latihan 1 – latihan1.py**

```python
from random import random
```

Baris ini **mengimpor fungsi `random()`** dari modul `random`.
Fungsi `random()` menghasilkan **bilangan acak** antara **0.0 sampai 1.0**.

---

```python
n = int(input("Masukkan nilai N: "))
```

* Program meminta pengguna memasukkan **N**, yaitu jumlah bilangan acak yang ingin ditampilkan.
* Nilai input diubah ke tipe **integer (int)**.

---

```python
i = 1
while i <= n:
```

* Variabel `i` digunakan sebagai **penghitung data ke-berapa**.
* Loop `while` berjalan selama `i` belum melebihi nilai `n`.

---

```python
    angka = random()
```

* Setiap iterasi menghasilkan **angka acak baru**.
* Angka ini berada di antara **0.0 dan 1.0**.

---

```python
    if angka < 0.5:
        print(f"data ke: {i} => {angka}")
        i += 1
```

* Hanya angka yang **lebih kecil dari 0.5** yang ditampilkan.
* Jika angka memenuhi syarat, program menampilkan:

  ```
  data ke: x => nilai
  ```
* Kemudian `i` ditambah 1.

---

```python


Cukup beri tahu!
