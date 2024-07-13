# Import pustaka yang diperlukan
import cv2
(Untuk baris ini bertujuan mengimport puataka opencv)

# Membaca gambar
image = cv2.imread('path/to/image.jpg')
(bertujuan untuk membaca gambar dari file yang disimpan di loksai dengan nama 'my foto.jpg')

# Menampilkan citra asli
cv2.imshow('Citra Asli', image)
cv2.waitKey(0)
(berfungsi untuk menampilkan gambar asli di jendela baru dengan judul "Citra Asli". Fungsi cv2.imshow() digunakan untuk menampilkan gambar di jendela, dan fungsi cv2.waitKey(0) digunakan untuk menunggu pengguna menekan tombol apa pun sebelum melanjutkan ke baris kode berikutnya.)

# Memutar citra
rotated_image = cv2.rotate(image, cv2.ROTATE_90_CLOCKWISE)
(untuk memutar gambar 90 derajat searah jarum jam. Konstanta cv2.ROTATE_90_CLOCKWISE digunakan untuk menentukan arah rotasi.)

# Menampilkan citra yang diputar
cv2.imshow('Citra Diputar', rotated_image)
cv2.waitKey(0)
( Baris kode ini untuk menampilkan gambar yang diputar di jendela baru dengan judul "Citra Diputar". )

# Mengubah ukuran citra
resized_image = cv2.resize(image, (256, 256))
( kode ini bertujuan untuk mengubah ukuran gambar menjadi 256x256 piksel. Parameter pertama adalah gambar yang ingin diubah ukurannya, dan parameter kedua adalah tupel yang berisi lebar dan tinggi baru gambar. ) 

# Menampilkan citra yang diubah ukurannya
cv2.imshow('Citra Diubah Ukuran', resized_image)
cv2.waitKey(0)
(menampilkan gambar yang diubah ukurannya di jendela baru dengan judul "Citra Diubah Ukuran".)

# Memotong citra
cropped_image = image[100:200, 100:200]
(untuk memotong bagian gambar dari koordinat (100, 100) ke koordinat (200, 200). Bagian gambar yang dipotong disimpan dalam variabel cropped_image.)

# Menampilkan citra yang dipotong
cv2.imshow('Citra Dipotong', cropped_image)
cv2.waitKey(0)
(kode ini menampilkan gambar yang dipotong di jendela baru dengan judul "Citra Dipotong".)

# Membalik citra
flipped_image = cv2.flip(image, 1)
( kode ini membalik gambar secara horizontal. Konstanta 1 digunakan untuk menentukan arah pembalikan (horizontal).)

# Menampilkan citra yang dibalik
cv2.imshow('Citra Dibalik', flipped_image)
cv2.waitKey(0)
(kode ini menampilkan gambar yang dibalik di jendela baru dengan judul "Citra Dibalik".)

# Menerjemahkan citra
translated_image = cv2.pyrUp(image)
(Baris kode ini menerjemahkan gambar dengan menggandakan ukurannya. Fungsi cv2.pyrUp() digunakan untuk menerjemahkan gambar.)

# Menampilkan citra yang diterjemahkan
cv2.imshow('Citra Diterjemahkan', translated_image)
cv2.waitKey(0)
(Baris kode ini menerjemahkan gambar dengan menggandakan ukurannya. Fungsi cv2.pyrUp() digunakan untuk menerjemahkan gambar.)

# Menutup semua jendela
cv2.destroyAllWindows()
(Baris kode ini menutup semua jendela yang dibuka oleh OpenCV.)
