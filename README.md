
# Deteksi Bentuk Gambar menggunakan Contour



## Teori Pendukung
Deteksi bentuk gambar menggunakan kontur (contour) adalah salah satu teknik yang digunakan dalam pengolahan citra untuk mengidentifikasi dan mengekstraksi objek atau bentuk dalam gambar. Kontur adalah garis lengkung yang menghubungkan titik-titik pada batas objek yang memiliki intensitas piksel yang sama atau serupa. Metode ini berguna dalam berbagai aplikasi seperti pengenalan pola, segmentasi objek, dan pengolahan gambar.

Proses deteksi bentuk gambar menggunakan kontur biasanya melibatkan beberapa langkah. Langkah pertama adalah mengubah gambar menjadi skala abu-abu (grayscale) untuk menghilangkan informasi warna dan memfokuskan pada informasi bentuk. Kemudian, dilakukan proses binarisasi untuk memisahkan objek dari latar belakang dengan mengubah intensitas piksel menjadi nilai biner berdasarkan suatu ambang batas.

Setelah gambar biner diperoleh, kontur pada gambar dapat diidentifikasi menggunakan teknik seperti algoritma "chain code" atau "contour tracing". Algoritma-algoritma ini melacak jalur piksel yang berdekatan untuk membentuk kurva yang menggambarkan batas objek. Kontur tersebut dapat ditemukan dengan menggunakan fungsi khusus dalam library pengolahan citra seperti OpenCV.

Selanjutnya, setelah kontur ditemukan, kita dapat melakukan berbagai operasi pada kontur yang terdeteksi. Misalnya, kita dapat menghitung luas kontur dengan menggunakan fungsi contourArea() untuk mendapatkan informasi tentang ukuran objek yang terdeteksi. Selain itu, kita juga dapat menggambar kotak pembatas (bounding box) menggunakan fungsi boundingRect() untuk menandai area yang diidentifikasi sebagai objek.

Deteksi bentuk gambar menggunakan kontur dapat digunakan dalam berbagai aplikasi. Misalnya, dalam pengenalan pola, kita dapat mengidentifikasi bentuk-bentuk khusus seperti lingkaran, segitiga, atau persegi untuk mengenali objek yang spesifik. Dalam segmentasi objek, teknik ini membantu memisahkan objek dari latar belakang dengan memanfaatkan perbedaan intensitas piksel pada batas objek. Hal ini sangat berguna dalam pemrosesan gambar medis, deteksi objek pada citra satelit, dan banyak lagi.

Dengan menggunakan OpenCV dan Python, proses deteksi bentuk gambar menggunakan kontur menjadi lebih mudah. OpenCV menyediakan berbagai fungsi dan metode yang mempermudah pengolahan citra, termasuk deteksi kontur. Dalam Python, kita dapat menggabungkan kemampuan OpenCV dengan kelebihan bahasa pemrograman Python untuk memanipulasi dan menganalisis data. Dalam lingkungan Jupyter Notebook, kita dapat dengan mudah menggabungkan kode, visualisasi, dan dokumentasi untuk memahami dan melacak proses deteksi bentuk gambar menggunakan kontur secara interaktif.

## Require

Sebelum menjalankan proyek ini, pastikan Anda memiliki hal-hal berikut terpasang di lingkungan Anda:

- Python 3.x
- Library OpenCV
- Library numpy
- Library matplotlib
- Jupyter Notebook


## Tahapan Penyelesaian Project
Berikut adalah langkah-langkah dalam mendeteksi bentuk gambar menggunakan kontur dengan menggunakan OpenCV dan Python di Jupyter Notebook:

#### 1. Persiapan Software:

- Memastikan Python dan OpenCV sudah terinstal di lingkungan Jupyter Notebook.

- Mengimpor library yang diperlukan, seperti cv2, numpy, dan matplotlib.

#### 2. Baca dan tampilkan gambar:

- Membaca gambar menggunakan OpenCV.

- Menampilkan gambar menggunakan Matplotlib untuk memeriksa apakah gambar telah terbaca dengan benar.

#### 3. Konversi gambar menjadi skala abu-abu:

- Mengubah gambar ke dalam skala abu-abu (grayscale)
    
- menggunakan fungsi cvtColor() dari OpenCV.

#### 4. Binarisasi gambar:

- Mengubah gambar menjadi citra biner dengan menggunakan metode thresholding. Misalnya, menggunakan thresholding adaptif untuk menghasilkan citra biner dengan ambang batas yang ditentukan secara otomatis.

#### 5. Temukan kontur pada gambar biner:

- Menggunakan fungsi findContours() dari OpenCV untuk menemukan kontur pada gambar biner.

- Kontur adalah garis yang menghubungkan titik-titik pada batas objek yang memiliki intensitas piksel yang sama atau serupa.

#### 6. Loop melalui setiap kontur dan lakukan operasi:

- Melakukan operasi pada setiap kontur yang ditemukan. Misalnya, menggambar kotak pembatas (bounding box) di sekitar setiap kontur atau menghitung luas kontur.

#### 7. Tampilkan gambar hasil:

- Menampilkan gambar hasil dengan kontur yang terdeteksi, menggunakan fungsi imshow() dari Matplotlib.

Dengan mengikuti tahapan-tahapan di atas, Anda dapat mengimplementasikan proyek deteksi bentuk gambar menggunakan kontur dalam Jupyter Notebook dengan menggunakan OpenCV dan Python.

## Cara menjalankan project ini

- Clone repository ini ke lingkungan lokal Anda atau unduh repository sebagai file ZIP dan ekstrak.
- Buka Jupyter Notebook di device Anda.
- Buka file PA_PC_202131116_FachrezaRiyanda_F.ipynb di Jupyter Notebook.
- Pastikan gambar yang ingin Anda deteksi bentuknya telah disiapkan dan berada di direktori yang sama dengan file Jupyter Notebook.
- Ikuti langkah-langkah yang dijelaskan dalam notebook untuk menjalankan proyek dan melihat hasil deteksi bentuk gambar menggunakan kontur.


## Jurnal Referensi

https://dspace.uii.ac.id/bitstream/handle/123456789/37125/05524019%20Meezan%20Khalil%20Gibran.pdf?sequence=1

## Referensi

Untuk informasi lebih lanjut tentang penggunaan OpenCV Python dan deteksi kontur, Anda dapat merujuk ke sumber-sumber berikut:

- Dokumentasi OpenCV: https://docs.opencv.org/

- Tutorial OpenCV di realpython.com: https://realpython.com/opencv-python-intro/

- Tutorial OpenCV di pyimagesearch.com: https://www.pyimagesearch.com/opencv-tutorials-resources-guides/
  
Hail deteksi (Output) :
![Output](https://github.com/Fachrezary/PA_PC_202131116_FachrezaRiyanda_F/assets/92991205/612713a6-3b38-40ad-a188-ddd00a0a0890)


## Authors

- [@Fachrezariyanda](https://github.com/Fachrezary)

