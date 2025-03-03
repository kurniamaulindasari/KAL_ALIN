---
title: 'Penyelesaian Sistem Persamaan '

---

# Penyelesaian Sistem Persamaan Linier
## Operasi Baris Elementer
Operasi Baris Elementer (OBE) adalah serangkaian manipulasi yang dapat dilakukan pada baris-baris suatu matriks untuk menyederhanakan atau mengubah bentuk matriks tersebut. Operasi baris elementer sangat penting dalam proses eliminasi Gauss dan eliminasi Gauss-Jordan, yang digunakan untuk menyelesaikan sistem persamaan linear dan menemukan invers matriks. Dengan melakukan serangkaian operasi baris elementer, kita dapat mengubah matriks menjadi bentuk eselon baris atau bentuk eselon baris tereduksi, yang lebih mudah untuk dianalisis dan diinterpretasikan.

### Terdapat tiga jenis operasi baris elementer:
1. Pertukaran Baris (Row Switching):
* Menukar posisi dua baris dalam matriks.
* Contoh: Jika kita memiliki matriks $A$, dan kita menukar baris ke-1 $(R_1)$, dengan baris ke-2 $(R_2)$ maka operasi ini dapat ditulis sebagai  $R_1$ &harr; $R_2$.
2. Perkalian Baris dengan Skalar (Row Scaling):
* Mengalikan suatu baris dengan skalar (bilangan) bukan nol.
* Contoh: Jika kita mengalikan baris ke-1 $(R_1)$, dengan skalar $k$, maka operasi ini dapat ditulis sebagai  $R_1$ &rarr; $kR_1$.
4. Penjumlahan Baris (Row Addition):
* Menambahkan kelipatan suatu baris ke baris lainnya.
* Contoh: Jika kita menambahkan $k$ kali baris ke-1 $(R_1)$ ke baris ke-2 $(R_2)$, maka operasi ini dapat ditulis sebagai $R_2$ &rarr; $R_2$ + $kR_1$.

## Eliminasi Gauss
Eliminasi Gauss adalah sebuah metode sistematis dalam aljabar linear yang digunakan untuk menyelesaikan sistem persamaan linear, mencari invers matriks, atau menentukan rank matriks.
#### Latihan Soal 1:

$$
\begin{array}{cc}
x_1+2x_2+3x_3&=6\\
2x_1+4x_2+6x_3&=12\\
x_3+x_2&=2
\end{array}
$$

#### Penyelesaian : 
* 
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
2 & 4 & 6 & | &12\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 0 & 0 & | &0\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{array}{cc}
x_2+x_3 = 2\\
x_2 = 2 - x_3\\
\end{array}
$$

* 
$$
\begin{array}{cc}
x_1+2x_2+3x_3 = 6\\
x_2 = 2 - x_3 \\
\end{array}
$$

* 
$$
\begin{array}{cc}
x_1 + 2(2-x_3)+3x_3 = 6\\
x_1 + 4-2x_3+3x_3 = 6\\
x_1+4+x_3\\
x_1=2-x_3
\end{array}
$$

* 
$$
\begin{array}{cc}
x_1 = 2-x_3\\
x_2=2-x_3\\
x_3=x_3
\end{array}
$$

* jadi hanya ada satu variabel maka sistem memiliki tak hingga banyak solusi.

#### Latihan Soal 2:
$$
\begin{array}{cc}
x_1+x_2+x_3&=3\\
2x_1+x_3&=5\\
x_1+2x_2&=3
\end{array}
$$
#### Penyelesaian : 
* 
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
2 & 0 & 2 & | &5\\
1 & 2 & 0 & | &3\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 1 & -1& | &0\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 0 & -1 & | &-1/2\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{array}{cc}
-x_3=-1/2\\
x_3=1/2
\end{array}
$$

* 
$$
\begin{array}{cc}
-2x_2=-1\\
x_2=1/2
\end{array}
$$

* 
$$
\begin{array}{cc}
x_1+x_2+x_3=3\\
x_1+1/2+1/2=3\\
x_1+1=3\\
x_1=2
\end{array}
$$

* hasil akhirnya adalah:
$$
\begin{array}{cc}
(x_1+x_2+x_3)=(2,1/2,1/2)
\end{array}
$$

* jadi, sistem ini memiliki *solusi tunggal*.



#### Latihan Soal 3:
$$
\begin{array}{cc}
x_1+x_2&=5\\
x_1+2x_3&=6\\
\end{array}
$$ 
#### Penyelesaian : 
* 
$$
\begin{bmatrix}
2 & 2 &  | &4\\
1 & 1 &  | &2\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{bmatrix}
1 & 1 &  | &2\\
1 & 1 &  | &2\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{array}{cc}
x_1+x_2=2\\
x_1=2-x_2\\
x_2=x_2
\end{array}
$$

* 
$$
\begin{array}{cc}
(x_1,x_2)=(2-x_2,x_2)
\end{array}
$$

* 
$$
\begin{array}{cc}
jika(x_2=0),maka((x_1,x_2)=(2,0))\\
jika(x_2=1),maka((x_1,x_2)=(1,1))\\
jika(x_2=2),maka((x_1,x_2)=(0,2))
\end{array}
$$

* maka sistem ini memiliki *tak hingga banyak solusi*.


#### Latihan Soal 4:
$$
\begin{array}{cc}
2x_1+2x_2&=4\\
x_1+x_2&=2\\
\end{array}
$$
#### Penyelesaian : 
* 
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 2 &| &6\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 1 &| &1\\
\end{bmatrix}
\quad
$$

* 
$$
\begin{array}{cc}
x_2=1\\
x_1+1=5\\
x_1=4
\end{array}
$$

* jadi:
$$
\begin{array}{cc}
(x_1,x_2)=(4,1)
\end{array}
$$

* maka, sistem ini memiliki *solusi tunggal*.