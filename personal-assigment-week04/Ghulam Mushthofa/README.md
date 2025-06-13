Tugas Individu – Klasifikasi Gambar Cicak vs Komodo dengan Transfer Learning
📌 Proyek ini merupakan implementasi klasifikasi dua jenis gambar objek, yaitu cicak dan komodo, menggunakan pendekatan transfer learning. Model yang digunakan adalah ResNet18 yang telah dilatih sebelumnya pada dataset ImageNet.

Tugas ini dibuat dalam rangka memenuhi penugasan mata kuliah [Nama Mata Kuliah].

🎯 Tujuan
Melatih model klasifikasi gambar dua objek secara efisien menggunakan transfer learning.

Menggunakan model pretrained (ResNet18) untuk menghemat waktu dan meningkatkan akurasi.

Mengevaluasi performa model dengan metrik klasifikasi seperti akurasi, confusion matrix, dan F1-score.

🖼️ Dataset
Jumlah total: 200 gambar

Kelas:

Cicak (100 gambar)

Komodo (100 gambar)

Sumber: dikumpulkan manual, terdiri dari berbagai sudut pengambilan dan pencahayaan

Struktur folder:

pets_cicak_komodo/
├── cicak/
└── komodo/

🛠️ Model & Teknik
Model: ResNet18 pretrained (ImageNet)

Strategi:

Membekukan seluruh layer kecuali fc

Fine-tuning hanya layer akhir

Augmentasi ringan: Resize, RandomHorizontalFlip

Framework: PyTorch

📊 Hasil & Evaluasi
Akurasi: ±91% (pada data validasi)

F1-score: ±0.90

Visualisasi:

Confusion matrix

Grafik akurasi dan loss per epoch

Classification report

📁 File di Repo Ini
cicak-klasifikasi-transfer-learning.ipynb – Notebook utama

laporan_tugas_individu.pdf – Laporan PDF maksimal 10 halaman

README.md – Deskripsi proyek ini

✍️ Refleksi Singkat
Selama mengerjakan tugas ini, saya belajar pentingnya struktur dataset, penggunaan model pretrained, dan bagaimana melakukan evaluasi model secara praktis. Kesalahan seperti penggunaan parameter pretrained=True berhasil saya atasi dengan mengganti ke weights=ResNet18_Weights.DEFAULT. Tugas ini memperkuat pemahaman saya terhadap transfer learning dan aplikasinya.

