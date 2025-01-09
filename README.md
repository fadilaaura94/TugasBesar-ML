![inima fix bgd](https://github.com/user-attachments/assets/4ab309da-fecb-4c3f-b3fb-fce25d77985a)

# TugasBesar-ML
Tugas Besar Pembelajaran Mesin - Klasifikasi Pola Konsumsi Obat dan Zat Tertentu Menggunakan Metode Random Forest

# Latar Belakang
Kecanduan terhadap zat tertentu, seperti kafein, alkohol, atau obat-obatan, merupakan tantangan signifikan bagi kesehatan masyarakat. Project ini memberikan prediksi atau klasifikasi menggunakan metode Random Forest mengenai pola konsumsi obat dan membantu dalam mengidentifikasi perilaku konsumsi pengguna.

# Tujuan Penelitian
Project ini bertujuan untuk membangun model klasifikasi yang dapat mengidentifikasi kemungkinan kecanduan seseorang terhadap zat tertentu berdasarkan faktor demografi dan psikologis.

# Metode Penelitian
Random forest adalah metode ansambel yang dirancang khusus untuk pengklasifikasian decision tree. Metode ini menggabungkan prediksi yang dibuat oleh beberapa decision tree, di mana setiap pohon dihasilkan berdasarkan nilai dari sekumpulan vektor acak yang independen. Metode ini menggabungkan kesederhanaan decision tree dengan fleksibilitas menghasilkan peningkatan akurasi yang sangat besar.

# Langkah Penelitian
1. Eksplorasi Data
   Memeriksa data awal, visualisasi distribusi, dan analisis korelasi data.
2. Prepocessing Data
   Transformasi target label, memilih dan normalisasi fitur, split dataset, dan visualisasi data target.
3. Pembuatan Model Baseline
   Membangun model dengan menggunakan parameter default tanpa tuning.
4. Eksplorasi Model
   Membangun model dengan menggunakan hyperparameter tuning dan eksplorasi model lainnya (AdaBoost dan XGBoost).
5. Evaluasi Model
   Mengevaluasi model dengan melihat metrik evaluasi (nilai accuracy, precision dan recall, serta (F1-Score) dan Confusion Matrix.

# Hasil dan Pembahasan
1. Empat model yang dianalisis untuk memprediksi kecanduan substansi:
   a) Random Forest (baseline),
   b) Random Forest dengan parameter tuning,
   c) AdaBoost, dan
   d) XGBoost.
3. Random Forest dengan hyperparameter tuning memiliki akurasi tertinggi, yaitu 84%, diikuti oleh Random Forest (baseline) dengan akurasi 83%, XGBoost dengan akurasi 82%, dan AdaBoost yang memiliki akurasi terendah, yaitu 82%.
4. Beberapa parameter yang digunakan untuk mengoptimalkan performa model di Random Forest dengan hyperparameter tuning antara lain: n_estimators, max_depth, min_samples_leaf, min_samples_split, dan random_state.
5. Semua model menunjukkan kinerja yang baik dalam mendeteksi kelas 1 (positif), namun kesulitan      dalam mendeteksi kelas 0 (negatif).
6. Hasil menunjukkan variasi fitur utama pada setiap model: 
   a) Fitur Oscore (Openness to Experience) menjadi yang paling berpengaruh pada Random Forest (baseline dan tuned).
   b) Pada AdaBoost, Fitur Escore (Extraversion) dominan, menunjukkan pengaruh interaksi sosial.
   c) Model XGBoost menempatkan Fitur Country (Negara) sebagai fitur utama, yang mencerminkan peran faktor geografis dan           budaya. 
