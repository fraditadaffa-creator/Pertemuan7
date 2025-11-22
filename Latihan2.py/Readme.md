
```python
modal = 100_000_000
```

Modal awal ditetapkan sebesar **100 juta rupiah**.

```python
total_laba = 0
```

Variabel untuk menyimpan **akumulasi total laba**.

---

```python
for bulan in range(1, 9):
```

Loop dari bulan 1 sampai bulan 8.

---

Bagian ini menentukan **persentase laba per bulan**:

```python
if bulan in [1, 2]:
    laba = 0
elif bulan in [3, 4]:
    laba = modal * 0.01
elif bulan in [5, 6, 7]:
    laba = modal * 0.05
elif bulan == 8:
    laba = modal * 0.03
```

Penjelasan:

* Bulan 1–2 >>> laba = 0
* Bulan 3–4 >>> laba = 1% × modal
* Bulan 5–7 >>> laba = 5% × modal
* Bulan 8 >>> laba = 3% × modal

---

```python
total_laba += laba
```

Laba bulan ini ditambahkan ke total laba.

```python
print(f"Laba bulan ke-{bulan} sebesar: {laba}")
```

Menampilkan laba tiap bulan.

---

```python
print("Total laba adalah:", total_laba)
```

Menampilkan total semua laba selama 8 bulan.



