# Alokasi-Memori
- Memori adalah perangkat keras yang digunakan untuk menyimpan informasi secara temporer atau permanen.
- Proses adalah program yang sedang dieksekusi. Proses biasanya terdiri dari process stack, yang memuat data temporer seperti parameter fungsi, return address, dan variable lokal.
- Alokasi memori yang akan dibicarakan adalah alokasi memori secara kontigu. Pada alokasi memori kontigu, setiap proses disimpan pada suatu bagian yang berlokasi bersebelahan dengan proses lainnya. Salah satu metode yang cukup sering digunakan dalam alokasi memori adalah membagi memori ke partisi-partisi yang mempunyai ukuran yang berbeda-beda (variable-partition). 
![image](https://user-images.githubusercontent.com/87927396/164263160-13c9f25d-d9c9-4a92-8a6e-c3e8dd41b6cc.png)

# Solusi Alokasi Memori
- First Fit
First fit adalah algoritma untuk alokasi memori yang mengalokasikan memori proses pada lubang pertama yang cukup. Pencarian biasanya dimulai dari lubang pertama. Pencarian akan berhenti ketika menemukan lubang pertama yang cukup.
- jika prosess masuk prosses 1 = 12, prosses2 = 10, prosses 3 = 9.
- ![image](https://user-images.githubusercontent.com/87927396/164264061-fd0b3700-6c90-4aa4-b942-4fa692cef809.png)

- Best Fit
Best fit adalah algoritma untuk alokasi memori yang mengalokasikan memori proses pada lubang cukup yang mempunyai ukuran terkecil. Best fit menginginkan agar alokasi menghasilkan lubang sisa yang paling kecil.
- jika prosess masuk prosses 1 = 12, prosses2 = 10, prosses 3 = 9.
- ![image](https://user-images.githubusercontent.com/87927396/164264655-fdd4f730-c1ea-43bb-86af-9d14a978b864.png)

- Worst Fit
Worst fit adalah algoritma untuk alokasi memori yang mengalokasikan memori proses pada lubang cukup yang mempunyai ukuran terbesar. Strategi ini akan menghasilkan lubang sisa yang besar. Diharapkan lubang sisa yang besar ini dapat digunakan untuk proses yang lain
- jika prosess masuk prosses 1 = 12, prosses2 = 10, prosses 3 = 9.
- ![image](https://user-images.githubusercontent.com/87927396/164264753-b6b7dd68-bba7-43ef-b762-fa4c64dd7588.png)

# kesimpulannya
setiap algoritma mempunyai keuntungan dan kerugian masing-masing. Algoritma first fit berjalan dengan cepat dan menghasilkan lubang yang cukup besar. Algoritma best fit tidak menyisakan lubang sama sekali. Algoritma worst fit menghasilkan lubang dengan ukuran terbesar. Dari segi waktu, algoritma first fit merupakan yang terbaik. Dari segi performansi, algoritma best fit merupakan yang terbaik karena tidak menyisakan lubang. Dari segi fragmentasi, algoritma worst fit merupakan yang terbaik karena menyisakan lubang yang besar. 
jadi, tidak ada algoritma yang terbaik. Penggunaan algoritma pada kasus yang salah akan menghasilkan hasil terburuk
