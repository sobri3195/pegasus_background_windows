## Pegasus Background Windows
Skrip Python ini secara otomatis mengunduh gambar acak dari Unsplash dan mengatur gambar tersebut sebagai wallpaper desktop pada sistem operasi Windows.

## Cara Menggunakan
Untuk menggunakan skrip ini, pastikan Python telah terinstal pada sistem Anda. Skrip ini memerlukan modul requests untuk menjalankan permintaan HTTP. Jika belum terinstal, Anda dapat menginstalnya menggunakan pip:
bash
Copy code
pip install requests

Setelah requests terinstal, Anda dapat menjalankan skrip dengan perintah berikut dari terminal atau command prompt:
bash
Copy code
python pegasus_background.py

## Cara Kerja
Skrip akan memulai dengan mengunduh gambar acak dari Unsplash menggunakan URL yang disediakan.
Gambar yang diunduh akan disimpan dengan nama random.jpg di direktori kerja saat ini.
Selanjutnya, skrip akan memeriksa apakah sistem operasi adalah versi 64-bit atau 32-bit untuk menyesuaikan cara pengaturan wallpaper.
Terakhir, gambar yang diunduh akan diatur sebagai wallpaper desktop menggunakan fungsi SystemParametersInfo dari Windows API.

## Fungsi
is_64bit(): Fungsi ini mengecek apakah sistem operasi adalah versi 64-bit atau 32-bit.
download(url, file_name): Fungsi ini mengunduh gambar dari URL yang diberikan dan menyimpannya dengan nama file yang ditentukan.
setup(pathtofile, version): Fungsi ini mengatur gambar yang diunduh sebagai wallpaper desktop. Parameter pathtofile adalah path ke file gambar, dan version adalah versi sistem operasi (64-bit atau 32-bit).

## Catatan
Pastikan Anda memiliki koneksi internet saat menjalankan skrip ini.
Hak cipta dari gambar yang diunduh milik fotografer di Unsplash.
