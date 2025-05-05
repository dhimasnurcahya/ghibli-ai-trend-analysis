🎥 Studio Ghibli AI Trend Analysis: Ethical Content Classification
📁 Proyek UTS Data Mining oleh Dhimas Nurcahya

Proyek ini menganalisis tren dan dampak konten AI bergaya Studio Ghibli di media sosial. Fokus utamanya adalah untuk mengklasifikasikan apakah sebuah konten mengandung isu etika atau tidak, menggunakan pendekatan machine learning (Naive Bayes dan Decision Tree). Data yang dianalisis mencakup metrik sosial (likes, shares, comments), parameter teknis (waktu generasi, ukuran file, pemakaian GPU), serta karakteristik tambahan seperti platform dan apakah gambar tersebut diedit secara manual.

📌 Tujuan Proyek
1. Mengidentifikasi pola tren dalam konten AI bergaya Studio Ghibli.
2. Menilai keterkaitan metrik sosial dan teknis dengan kemungkinan munculnya isu etika.
3. Membangun model klasifikasi untuk mendeteksi konten bermasalah secara etika.
4. Membandingkan performa dua algoritma klasifikasi: Naive Bayes dan Decision Tree.

📊 Dataset
Dataset yang digunakan adalah ai_ghibli_trend_dataset_v2.csv, berisi kumpulan konten bergaya AI-Ghibli dan informasi metadata sosial dan teknis.

Fitur Utama:
1. likes, shares, comments
Jumlah interaksi pengguna di media sosial.
2. generation_time	Waktu (dalam detik)
untuk menghasilkan gambar.
3. gpu_usage
Jumlah penggunaan GPU (dalam %).
4. file_size_kb
Ukuran gambar yang dihasilkan dalam KB.
5. style_accuracy_score
Seberapa mirip gambar dengan gaya Ghibli (0–1).
6. platform
Platform distribusi (misal: Instagram, Twitter).
7. is_hand_edited
Apakah gambar telah diedit secara manual (Yes/No).
8. ethical_concerns_flag
Apakah konten ini menimbulkan kekhawatiran etika (Yes/No). → label target

🧰 Tools & Libraries
1. Python 3
2. Google Colab
3. Pandas, NumPy – manipulasi data
4. Matplotlib, Seaborn – visualisasi
5. Scikit-Learn – preprocessing, model, evaluasi

📁 Struktur Analisis
1. Import Library
Meload semua dependensi Python yang dibutuhkan.
2. Read Dataset
Membaca dan menampilkan struktur dataset untuk pemahaman awal.
3. Handling Missing Values
Mengisi nilai kosong (jika ada) pada kolom numerik menggunakan median dan kategorikal menggunakan modus.
4. Visualisasi Data
- Distribusi likes, shares, dan comments.
- Korelasi antar fitur numerik.
- Perbandingan jumlah konten etis dan tidak etis per platform.
5. Train the Model
- Melakukan label encoding untuk data kategorikal.
- Membagi dataset menjadi data latih dan uji.
- Melatih dua model: Naive Bayes dan Decision Tree.
6. Predict and Evaluate
- Melakukan prediksi menggunakan kedua model.
- Menghitung akurasi dan membuat classification report.
- Menampilkan confusion matrix untuk evaluasi visual.

🧪 Hasil Evaluasi
Model	          Akurasi (%)	Precision	Recall	F1-Score
Naive Bayes	    XX.XX	        ...	     ...	    ...
Decision Tree   YY.YY	        ...	     ...	    ...
Gantilah XX.XX dan YY.YY dengan hasil akurasi Anda dari Google Colab.

🔍 Insight Utama
- Konten yang diedit manual memiliki kecenderungan lebih tinggi untuk tidak menimbulkan isu etika.
- Platform tertentu menunjukkan frekuensi lebih besar dalam konten bermasalah.
- Fitur sosial seperti jumlah likes dan shares tidak selalu mencerminkan apakah suatu konten menimbulkan kekhawatiran etis.
- Decision Tree cenderung memberikan hasil klasifikasi yang lebih baik dibandingkan Naive Bayes untuk dataset ini.

📌 Kesimpulan
Model klasifikasi seperti Naive Bayes dan Decision Tree efektif dalam memprediksi isu etika pada konten AI. Visualisasi dan korelasi fitur juga memberikan insight penting bagi pengawasan dan regulasi konten AI di masa depan.

🧾 Lisensi & Penggunaan
Proyek ini dibuat sebagai bagian dari UTS Data Mining dan hanya untuk keperluan pembelajaran dan akademik. Tidak diperuntukkan untuk penggunaan komersial.
