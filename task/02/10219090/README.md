# 10219090
Difa Ayatullah Muthmainnah


## materi sebelumnya
1. Penyelesaian rekursif
2. Metode penyelesaian persamaan differensial (cth: double spring, osilasi teredam, predator-prey) menggunakan:
- Simple Euler
- Runge Kutta
3. Monte carlo
4. Penyelesaian persamaan differensial parsial (cth: dispersi suhu)
5. Fourier transform:
- DFT (Discrete Fourier Transform) yang dapat dilakukan dengan FFT (Fast Fourier Transform)



## materi paling menarik
Menurut saya, materi yang paling menarik adalah metode penyelesaian persamaan differensial karena problem ini sering ditemui dalam penyelesaian permasalahan fisis. 
Berbagai sistem fisis yang dijumpai seperti double spring, osilasi teredam, fluida menggunakan bernoulli adalah beberapa contoh yang memiliki solusi
permasalahan dalam bentuk persamaaan differensial. Penyelesaian secara analitik cukup sulit untuk dilakukan karena melibatkan banyak metode matematika yang
perlu dipahami sehingga penggunaan model numerik seperti python sangat memudahkan.


## materi paling membosankan
Untuk materinya sebenarnya menurut saya cukup menarik dan tidak membosankan. Hanya saja mungkin ketika masuk kepada penjelasan yang banyak dan praktik coding
yang sedikit, menjadi agak bosan.

## materi yang sudah dipami
Saya agak sulit memahami coding karena basicnya yang belum kuat dari segi python sehingga yang masih terkejar sekitar materi-materi awal sampai monte carlo.


## materi yang belum dipahami
Di bagian akhir seperti fourier transform saya sudah tidak paham peruntukannya dalam sistem fisis jadi ingin memahaminya.


## contoh program
```python
# contoh program python Discrete Fourier Transform (DFT) 
import numpy as np
import matplotlib.pyplot as plt

def DFT(x):
    N = x.size
    n = np.arange(N)
    k = n.reshape((N,1))
    e = np.exp(-2j * np.pi * k * n / N)
    return np.dot(e, x)

t = np.arange(0.0, 1.0, 0.01)

frek = 1
sinyal = np.sin(2*np.pi*frek*t)
# sinyal = np.sin(20 * 2 * np.pi * t) + 0.5 * np.sin(40 * 2 * np.pi * t)
# sinyal = np.sin(20 * 2 * np.pi * t) + 0.5 * np.sin(40 * 2 * np.pi * t) + 0.5 * np.sin(70 * 2 * np.pi * t)

plt.plot(sinyal)
plt.show()

#Hasilnya adalah
<img width="283" alt="image" src="https://user-images.githubusercontent.com/81822571/196590958-3dbc2e36-9436-4c1d-b8be-53db5114dac7.png">


## cara perkuliahan
Sebenernya sejauh ini sudah bagus menurut saya. Mungkin ditambahkan lebih banyak kerja mandiri.

## topik sistem fisis
Menurut saya yang menarik saat ini yaitu fisika yang berkaitan dengan perilaku cahaya misalnya efek dan fenomena fotolistrik.


## simulasi dan visualisasi
Sangat tertarik. Menurut saya hal yang menarik untuk disimulasikan ataupun divisualisasikan adalah hal-hal yang mikroskopis seperti topik getaran kristal,
ataupun topik lain yang sedang dipelajari di matkul baru di semester ini. Hal ini akan menjadi menarik karena merasa relate dengan apa yang sedang dibahas
dan bisa menambah konsep pemahaman karena visualisasi hal yg mikroskopik sering kali tidak terbayang karena tidak bisa ditemukan di kehidupan nyata
secara kasat mata.
