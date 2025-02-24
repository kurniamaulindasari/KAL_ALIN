---
title: 'Penyelesaian Sistem Persamaan '

---

## Penyelesaian Sistem Persamaan Linier
### Operasi Baris Elementer
### Eliminasi Gauss
Contoh Soal 1:
Selesaikan dengan menggunakan Eliminasi Gaus
$$
\begin{array}{cc}
x_1+2x_2+3x_3z&=6\\
2x_1+4_2+6x_12&=4\\
x_3-x_2&=2
\end{array}
$$


Latihan Soal 1:
$$
\begin{array}{cc}
x_1+2x_2+3x_3&=6\\
2x_1+4x_2+6x_3&=12\\
x_3+x_2&=2
\end{array}
$$
Penyelesaian : 
* matriks augmentasi
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
2 & 4 & 6 & | &12\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$
* Eliminasi koefisien utama pada baris kedua
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 0 & 0 & | &0\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$
* Tukar baris kedua dan ketiga
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 1 & 1 & | &2\\
0 & 0 & 0 & | &0\\
\end{bmatrix}
\quad
$$
* Eliminasi koefisien $x_2$ pada baris pertama
$$
\begin{bmatrix}
1 & 0 & 1 & | &2\\
0 & 1 & 1 & | &2\\
0 & 0 & 0 & | &0\\
\end{bmatrix}
\quad
$$
* 
$$
\begin{array}{cc}
x_1+x_3&=2\\
x_2+x_3&=2\\
\end{array}
$$
* 
$$
\begin{array}{cc}
x_1&=2-1&=1\\
x_2&=2-1&=1\\
x_3&=1\\
\end{array}
$$
* jadi hasilnya 
$$
\begin{array}{cc}
x_1&=1\\
x_2&=1\\
x_3&=1\\
\end{array}
$$

Latihan Soal 2:
$$
\begin{array}{cc}
x_1+x_2+x_3&=3\\
2x_1+x_3&=5\\
x_1+2x_2&=3
\end{array}
$$
Penyelesaian : 



Latihan Soal 3:
$$
\begin{array}{cc}
x_1+x_2&=5\\
x_1+2x_3&=6\\
\end{array}
$$ 
Penyelesaian : 



Latihan Soal 4:
$$
\begin{array}{cc}
2x_1+2x_2&=4\\
x_1+x_2&=2\\
\end{array}
$$
Penyelesaian : 
