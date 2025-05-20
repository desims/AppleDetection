# Selamat datang di Blog AI & Data Science Sel!

Blog ini berisi konten seputar AI, Data Science, dan contoh-contoh kode Python.

Implementasi pertama tanpa merubah konsep dasar dari teknik sama sekali, menghasilkan model yang baik untuk warna merah dan gagal untuk warna kuning dan hijau

## Percobaan pertama hsv+red mask

```python
# Konversi ke HSV
image_hsv = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2HSV)

# Rentang warna merah apel dalam HSV (pakai np.array untuk inRange)
low_apple_red = np.array([160, 153, 153], dtype=np.uint8)
high_apple_red = np.array([180, 255, 255], dtype=np.uint8)
```

![image](https://github.com/user-attachments/assets/476a9b1e-c5a3-486a-9fea-26d25e9d6992)

---

```python
## Percobaan pertama hsv+red mask+ other color mask
# Konversi ke HSV
image_hsv = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2HSV)

# Rentang warna merah apel dalam HSV (pakai np.array untuk inRange)
low_apple_red = np.array([160, 153, 153], dtype=np.uint8)
high_apple_red = np.array([180, 255, 255], dtype=np.uint8)

low_apple_raw = np.array([0, 150, 150], dtype=np.uint8)
high_apple_raw = np.array([15, 255, 255], dtype=np.uint8)

# Orange-kekuningan
low_orange = np.array([11, 100, 100])
high_orange = np.array([25, 255, 255])

# Kuning
low_yellow = np.array([26, 80, 80])
high_yellow = np.array([35, 255, 255])

# Hijau muda ke hijau tua (gradasi apel hijau)
low_green = np.array([36, 60, 60])
high_green = np.array([85, 255, 255])
```
![image](https://github.com/user-attachments/assets/6edf1a1e-adea-4e84-ae7c-4766126fd85f)

---

