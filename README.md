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
![Screenshot 2024-10-27 221148](https://github.com/user-attachments/assets/cb6bcf90-51b7-4c33-9071-4dad6bf6a620)

#Menampilkan total biaya jika tiket valid
if total_tiket > 0:
    print(f"Jumlah yang harus dibayar: Rp{jumlah_bayar:.0f}")

Penjelasan:

### Menampilkan Hasil:

Program memeriksa apakah total_tiket lebih dari 0 untuk memastikan bahwa tiket yang valid telah dipilih.

Jika valid, program mencetak jumlah yang harus dibayar. Format output menggunakan f-string untuk menyajikan total dalam format yang rapi, tanpa desimal, menggunakan {jumlah_bayar:.0f}.


## FlowChart
![ss17](https://github.com/user-attachments/assets/a2ac0a5d-0e50-40e8-8044-59f01b1741ad)



## KALKULATOR SEDERHANA


![Screenshot 2024-10-27 231053](https://github.com/user-attachments/assets/3912ceac-f730-469f-a81b-6f6a1cf6d8d5)
### 1. Input Angka Pertama

Baris: angka1 = float(input("Masukkan angka pertama: "))

Fungsi:

input("Masukkan angka pertama: "): Menampilkan pesan kepada pengguna untuk memasukkan angka pertama. Fungsi ini menunggu hingga pengguna mengetikkan input dan menekan Enter.

float(...): Mengonversi input yang diterima (yang merupakan string) menjadi tipe data float. Ini memungkinkan pengguna untuk memasukkan angka desimal.

angka1: Variabel ini menyimpan nilai angka pertama yang dimasukkan oleh pengguna.



### 2. Input Angka Kedua

Baris: angka2 = float(input("Masukkan angka kedua: "))

Fungsi:

Proses ini mirip dengan langkah sebelumnya. Pengguna diminta untuk memasukkan angka kedua.

angka2: Variabel ini menyimpan nilai angka kedua yang dimasukkan.



### 3. Input Operator

Baris: operator_input = input("Masukkan operator (+, -, *, /): ").strip()

Fungsi:

input("Masukkan operator (+, -, *, /): "): Menampilkan pesan untuk meminta pengguna memilih salah satu operator aritmatika (penjumlahan, pengurangan, perkalian, atau pembagian).

.strip(): Menghapus spasi di awal dan akhir string yang dimasukkan oleh pengguna. Ini berguna untuk memastikan bahwa hanya karakter penting yang tersisa untuk pemrosesan lebih lanjut.

operator_input: Variabel ini menyimpan operator yang dimasukkan oleh pengguna.


## Menghitung Hasil Berdasarkan Operator
![Screenshot 2024-10-27 231126](https://github.com/user-attachments/assets/522ae3da-5fea-46da-a145-7544e9b15714)


### Bagian kode ini bertugas untuk menentukan operasi aritmatika berdasarkan input operator dari pengguna.

Pertama, program memeriksa apakah operator adalah penjumlahan (+). Jika benar, hasil penjumlahan dari angka1 dan angka2 disimpan dalam variabel hasil.
Jika operator adalah pengurangan (-), program melakukan pengurangan dan menyimpan hasilnya.
Untuk perkalian (*), program melakukan operasi perkalian dan menyimpan hasilnya di variabel yang sama.
Ketika operator adalah pembagian (/), program memeriksa apakah angka2 bukan nol. Jika tidak nol, program melakukan pembagian; jika nol, program menyimpan pesan kesalahan tentang pembagian dengan nol.
Jika operator yang dimasukkan tidak valid (bukan salah satu dari empat operator aritmatika), program menyimpan pesan kesalahan yang sesuai.
Tujuan dari kode ini adalah untuk melakukan operasi yang tepat dan memberikan umpan balik jika terjadi kesalahan, seperti pembagian dengan nol atau penggunaan operator yang tidak valid.

## Menampilkan Hasil
![Screenshot 2024-10-27 231153](https://github.com/user-attachments/assets/db0dd605-1e41-4408-859f-c8c0e13cf3a5)

### Tujuan: Menampilkan hasil perhitungan kepada pengguna.

### Proses:
Menggunakan print() untuk menampilkan hasil.
Memanfaatkan f-string (f"Hasil: {hasil}") untuk format yang lebih bersih dan jelas.


## FLOWCHART

![FLOWCHART 2](https://github.com/user-attachments/assets/6c4fa9ab-5fa0-4c20-bec1-6b1e2c4193c4)



