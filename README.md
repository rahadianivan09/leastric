
# 🔌 Leastric - Energy Monitoring MVP

Leastric adalah sebuah aplikasi dashboard ringan berbasis Streamlit untuk memantau konsumsi listrik, memprediksi beban listrik ke depan, dan mengenali pola perangkat melalui pendekatan Machine Learning.

## 🚀 Fitur Utama

- 📈 Visualisasi konsumsi listrik harian
- 🔮 Prediksi konsumsi listrik 7 hari ke depan (dengan Prophet)
- 🧠 Clustering pola konsumsi berdasarkan jam (KMeans)
- 📂 Mendukung upload data CSV sendiri atau gunakan data demo

## 📊 Contoh Use Case

Aplikasi ini cocok untuk:
- Rumah tangga pintar yang ingin tahu kapan perangkat menyedot listrik paling tinggi
- Perusahaan untuk analisis efisiensi konsumsi
- Edukasi dan showcase MVP energi berbasis data

## 🖼️ Tampilan Aplikasi

![screenshot](screenshot.png) <!-- bisa diganti nanti sesuai gambar kamu -->

## 📁 Struktur Proyek

```
leastric/
│
├── data/
│   └── dummy_energy.csv      # Data simulasi (dummy)
├── app.py                    # Main Streamlit app
├── requirements.txt          # Dependensi Python
└── README.md                 # Dokumentasi proyek
```

## 🛠️ Cara Menjalankan (Local)

1. Clone repo ini:
   ```bash
   git clone https://github.com/rahadianivan09/leastric.git
   cd leastric
   ```

2. Buat dan aktifkan environment (opsional):
   ```bash
   python -m venv env
   source env/bin/activate  # atau `env\Scripts\activate` di Windows
   ```

3. Install dependensi:
   ```bash
   pip install -r requirements.txt
   ```

4. Jalankan aplikasi:
   ```bash
   streamlit run app.py
   ```

5. Upload file CSV sendiri atau centang "Gunakan dummy data" di sidebar.

## 🧠 Teknologi yang Digunakan

- [Streamlit](https://streamlit.io/)
- [Prophet](https://facebook.github.io/prophet/) untuk forecasting
- [Scikit-Learn](https://scikit-learn.org/) untuk clustering
- [Matplotlib & Seaborn](https://matplotlib.org/) untuk visualisasi

## 📌 Catatan

- Data yang digunakan adalah data simulasi (dummy).
- Untuk penggunaan nyata, sistem ini bisa diintegrasikan dengan data logger / IoT device melalui format CSV.

## 🙋 Kontributor

> Dibuat oleh [@rahadianivan09](https://github.com/rahadianivan09)  
> Dengan dukungan teknikal dan desain dari ChatGPT OpenAI

---

## 📜 Lisensi

Open Source – Bebas digunakan untuk edukasi & pengembangan lebih lanjut.
