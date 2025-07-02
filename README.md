# SegmentationMachineLearning

Proyek ini merupakan aplikasi berbasis Streamlit untuk melakukan segmentasi pelanggan mall menggunakan algoritma *K-Means* dan *Hierarchical Clustering*. Analisis segmentasi ini membantu memahami perilaku belanja pelanggan berdasarkan data yang diunggah.

## Fitur

- Upload dataset pelanggan dalam format CSV
- Pra-pemrosesan otomatis (menghapus kolom ID, encoding gender)
- Pilihan fitur yang digunakan untuk clustering
- Pilihan algoritma: K-Means atau Hierarchical Clustering
- Visualisasi hasil clustering (scatter plot 2D)
- Visualisasi dendrogram untuk Hierarchical Clustering
- Evaluasi clustering (Silhouette Score, Inertia/SSE)
- Elbow Method untuk menentukan jumlah cluster optimal (K-Means)
- Download hasil clustering dalam format CSV

## Cara Menjalankan

````markdown
1. **(Opsional)** Buat virtual environment (venv) baru:

   ```bash
   python -m venv venv
   ```

   Aktifkan venv:

   - **Windows:**  

     ```bash
     venv\Scripts\activate
     ```

   - **Mac/Linux:**  

     ```bash
     source venv/bin/activate
     ```

2. Install dependensi yang diperlukan:

   ```bash
   pip install -r requirements.txt
   ```

3. Jalankan aplikasi dengan perintah:

   ```bash
   streamlit run main.py
   ```

4. Buka browser dan akses alamat yang ditampilkan (<http://localhost:8501>).

5. Upload dataset dalam format CSV.

6. Pilih fitur dan algoritma clustering sesuai kebutuhan.

7. Analisis hasil segmentasi dan download hasilnya jika diperlukan.

## Struktur Dataset

Dataset yang digunakan memiliki kolom berikut:

- CustomerID (ID pelanggan, akan dihapus otomatis)
- Gender (jenis kelamin, akan di-encode otomatis)
- Age (umur pelanggan)
- Annual Income (k$) (pendapatan tahunan dalam ribuan dolar)
- Spending Score (1-100) (skor pengeluaran pelanggan)

Pastikan dataset memiliki format header dan urutan kolom seperti di atas untuk kompatibilitas maksimal.

```
