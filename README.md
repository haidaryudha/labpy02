#  LAPORAN PRAKTIKUM 2
## PROGRAM PEMESANAN TIKET
### KODE PROGRAM

### Inisialisasi Harga Tiket:
![Screenshot 2024-10-27 212959](https://github.com/user-attachments/assets/2a726a78-ed23-45c6-bbe7-038764239c5a)


Dua variabel,harga_tiket_reguler dan harga_tiket_vip, ditetapkan untuk menyimpan harga masing-masing jenis tiket.
Tiket reguler dihargai Rp50.000 dan tiket VIP Rp100.000.
Dengan menggunakan variabel ini, kita dapat dengan mudah mengubah harga tiket di satu tempat tanpa harus mencarinya di seluruh kode.


### Mengambil Input Penguna :
![Screenshot 2024-10-27 211704](https://github.com/user-attachments/assets/76a7b9bd-85ce-4bbf-858c-b86bdc529090)

### Meminta Input dari Pengguna:
Program menggunakan fungsi
input() untuk menerima data dari 
pengguna.

### Tipe Tiket:
Pengguna diminta untuk
memilih jenis tiket yang diinginkan,
apakah reguler atau VIP.

### Status Anggota:
Pengguna juga harus 
menyatakan apakah mereka
memiliki kartu anggota.


Informasi ini disimpan dalam dua
variabel: tipe_tiket_input dan
status_member_input.


### Proses Pengolahan Input:
.strip(): Menghapus spasi di awal dan akhir input untuk mencegah kesalahan.

.lower(): Mengonversi semua huruf menjadi huruf kecil untuk konsistensi, sehingga input "Reguler" dan "reguler" dianggap sama.


### Menghitung Biaya Tiket
![Screenshot 2024-10-27 213057](https://github.com/user-attachments/assets/a7af5704-fa82-41f5-aed9-77c40c83a993)

### Logika Penentuan Harga Tiket:
* Menggunakan struktur kontrol if-elif-else, program menentukan harga tiket berdasarkan input pengguna.

* Jika pengguna memilih "reguler", total_tiket diatur ke harga tiket reguler.

* Jika memilih "VIP", total_tiket diatur ke harga tiket VIP.

* Jika input tidak sesuai, program mencetak pesan kesalahan dan mengatur total_tiket menjadi 0 untuk menunjukkan input tidak valid.


### Pentingnya Validasi Input:
Validasi ini sangat krusial untuk memastikan bahwa program hanya melanjutkan dengan data yang benar, sehingga mencegah kesalahan dalam perhitungan dan kesalahan lainnya.


### MengHitung Diskon
![Screenshot 2024-10-27 220545](https://github.com/user-attachments/assets/586729ee-63ba-4e42-8069-f32eee43b051)

Baris pertama kode ini menggunakan operator ternary untuk menetapkan nilai diskon_member. Jika pengguna menjawab "ya" ketika ditanya tentang kepemilikan kartu anggota, maka diskon_member akan diatur menjadi 0.2, yang menunjukkan bahwa pengguna berhak mendapatkan diskon sebesar 20%. Jika pengguna menjawab "tidak", maka diskon_member akan diatur menjadi 0, yang berarti tidak ada diskon yang diterapkan. Dengan cara ini, program secara otomatis menyesuaikan tingkat diskon berdasarkan input pengguna.


### Menghitung Total Pembayaran:

Pada baris kedua, total pembayaran, yang disimpan dalam variabel jumlah_bayar, dihitung dengan mengalikan total_tiket dengan (1 - diskon_member). Ini berarti bahwa jika pengguna memiliki diskon, harga akhir akan berkurang sesuai dengan persentase diskon.

Sebagai contoh, jika harga tiket adalah Rp50.000 dan pengguna berhak atas diskon 20%, maka total yang harus dibayar menjadi Rp40.000, dihitung sebagai Rp50.000 dikalikan 0.8 (yaitu 1 - 0.2).


### Menampilkan hasil









