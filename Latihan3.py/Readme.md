
# 📌 **Penjelasan Baris Per Baris**

```python
saldo = 1_000_000
```

Mengatur saldo awal ATM menjadi **1 juta rupiah**.

---

```python
while True:
```

Loop **tak terbatas**, akan berhenti jika `break`.

---

Menu ditampilkan:

```python
print(f"\nSaldo saat ini: Rp {saldo}")
print("1. Tarik Uang")
print("2. Keluar")
```

---

User memilih menu:

```python
menu = input("Pilih menu (1/2): ")
```

---

## **Jika user memilih opsi 1 (tarik uang)**

```python
if menu == "1":
    tarik = int(input("Masukkan jumlah penarikan: "))
```

Meminta jumlah uang yang ingin ditarik.

---

### **Cek apakah saldo cukup**

```python
if tarik <= saldo:
    saldo -= tarik
    print("Penarikan berhasil!")
else:
    print("Saldo tidak cukup!")
```

Jika cukup, saldo dikurangi. Jika tidak, tampilkan pesan gagal.

---

### **Cek apakah saldo sudah habis**

```python
if saldo == 0:
    print("Saldo habis. Terima kasih telah menggunakan ATM!")
    break
```

Jika saldo = 0, program berhenti.

---

## **Jika user memilih opsi 2 (keluar)**

```python
elif menu == "2":
    print("Terima kasih telah menggunakan ATM!")
    break
```

Program selesai.

---

## **Jika menu salah**

```python
else:
    print("Menu tidak valid, coba lagi.")
```
