# Selamat datang di Blog AI & Data Science Sel!

Blog ini berisi konten seputar AI, Data Science, dan contoh-contoh kode Python.

Implementasi pertama tanpa merubah konsep dasar dari teknik sama sekali, menghasilkan model yang baik untuk warna merah dan gagal untuk warna kuning dan hijau

## Contoh Konversi Warna ke HSV

```python
# Konversi ke HSV
image_hsv = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2HSV)

# Rentang warna merah apel dalam HSV (pakai np.array untuk inRange)
low_apple_red = np.array([160, 153, 153], dtype=np.uint8)
high_apple_red = np.array([180, 255, 255], dtype=np.uint8)


![image](https://github.com/user-attachments/assets/476a9b1e-c5a3-486a-9fea-26d25e9d6992)

---
