### TUGAS-3-ML Pertemuan 11 ANN

### Menyiapkan environment

1. Install virtualenv:

    ```bash
    pip install virtualenv
    ```

2. Membuat environtment menggunakan virtualenv:

    ```bash
    virtualenv env
    ```

3. Mengaktifkan environtment menggunakan virtualenv:

    ```bash
    ./env/Script/activate
    ```

### Membuat clone repo ini
    
    git clone https://github.com/Fanul1/2108107010029_Pertemuan_11_ANN

Selanjutnya

    cd 2108107010029_Pertemuan_11_ANN

### Instalasi librari yang diperlukan
1. Instal librari yang ada dari file `requirements.txt`:
    pip install -r requirements.txt

2. Perlu dicatat bahwa librari yang digunakan bergantung pada librari yang lainnya.

### ANN - Klasifikasi

Dataset yang saya ambil dari kaggle berikut linknya : https://www.kaggle.com/datasets/bhavikjikadara/loan-status-prediction/data

Deskripsi : Pada dataset Prediksi Status Pinjaman ini kami memiliki data pemohon yang sebelumnya mengajukan pinjaman berdasarkan properti yang merupakan Pinjaman Properti. Bank akan memutuskan apakah akan memberikan pinjaman kepada pemohon berdasarkan beberapa faktor seperti Applicant Income, Loan Amount, previous Credit History, Co-applicant Income, dan lain-lain

Menggunakan tahapan dari Tugas 2 sebelumnya namun menggunakan model yang berbeda yakni ANN menggunakan librari dari Tensorflow dengan :
 * Total params: 781 (3.05 KB)
 * Trainable params: 781 (3.05 KB)
 * Non-trainable params: 0 (0.00 B)

Diperoleh skor untuk
 * Training Accuracy: 0.9547169804573059
 * Test Accuracy: 0.8314606547355652

### ANN - Regresi

Dataset yang saya ambil dari kaggle berikut linknya : https://www.kaggle.com/datasets/sumitm004/forest-fire-area. 

Deskripsi : Kumpulan data tersebut berisi 517 kebakaran di taman alam Montesinho di Portugal. Setiap kejadian hari kerja, bulan, koordinat, dan luas lahan yang terbakar dicatat, serta beberapa data meteorologi seperti hujan, suhu, kelembaban, dan angin. Alur kerja membaca data dan melatih model regresi berdasarkan variabel spasial, temporal, dan cuaca.

Menggunakan tahapan dari Tugas 2 sebelumnya namun menggunakan model yang berbeda yakni ANN menggunakan librari dari Tensorflow dengan :
 * Total params: 1,445 (5.65 KB)
 * Trainable params: 481 (1.88 KB)
 * Non-trainable params: 0 (0.00 B)
 * Optimizer params: 964 (3.77 KB)

Diperoleh skor Mean Squared Error (MSE) :  1.825542535518884

### Hasil perbandingan dengan ANN dengan SVM (SVC & SVR)
1. Dari hasil pada file ANN-klasifikasi.ipynb diperoleh bahwasanya akurasi tidak berbeda jauh dengan yang ada pada SVCnya yakni selisihnya 7% atau 0.08. Dimana untuk ANN 0.83 atau 83% sedangkan untuk SVC 77% atau 0.77.
2. Dari hasil pada file ANN-regresi.ipynb diperoleh bahwasanya skor MSE nya 1.825542535518884 sedangkan pada SVR Mean Squared Error :  1.9438843129613104 berarti semakin kecil nilai, semakin baik dikarenakan bobot lebih besar pada pencilan.

### Kesimpulannya dari perbandingan antara Tugas ini dengan Tugas sebelumnya khusus pada kedua kasus dataset diatas dapat diketahui bahwa ANN lebih baik daripada SVM.
 
Note :
* Untuk Tugas 2 sebelumnya berikut ini: https://github.com/Fanul1/TUGAS-2-ML bila membutuhkan detail analysis untuk EDAnya dikarenakan memiliki tahapan yang sama namun library yang digunakan berbeda.
* Menggunakan versi libraries yang bisa dapat merubah hasil output yang ada sebelumnya.