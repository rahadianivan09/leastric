
## ⚡ Leastric – Energy Monitoring & Prediction Dashboard

Leastric adalah aplikasi dashboard berbasis **Streamlit** untuk **monitoring konsumsi listrik**, **prediksi beban listrik 7 hari ke depan**, dan **pengenalan pola perangkat** menggunakan teknik **machine learning (clustering)**.

### 🔧 Fitur Utama

- ✅ Upload data CSV konsumsi listrik per timestamp
- ✅ Opsi menggunakan **dummy dataset** bawaan (`dummy_energy.csv`)
- 📊 Visualisasi **total konsumsi listrik harian**
- 🔮 Prediksi konsumsi listrik **7 hari ke depan** menggunakan **Prophet**
- 🧠 **Clustering pola perangkat** berdasarkan konsumsi per jam (KMeans)
- 📥 Download hasil prediksi dan clustering dalam format CSV

---

### 📂 Struktur Folder

```bash
.
├── app.py                    # Main Streamlit App
├── requirements.txt          # Dependency file untuk deploy
├── data/
│   └── dummy_energy.csv      # Contoh dataset demo
├── outputs/
│   ├── forecast_output.csv   # Hasil prediksi (auto-generated)
│   └── cluster_output.csv    # Hasil clustering (auto-generated)
└── README.md                 # Deskripsi proyek (file ini)
```

---

### 🚀 Cara Menjalankan Secara Lokal

1. Clone repo ini:

```bash
git clone https://github.com/rahadianivan09/leastric.git
cd leastric
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Jalankan aplikasi:

```bash
streamlit run app.py
```

---

### 📦 Dependencies Utama

- `streamlit`
- `pandas`, `matplotlib`, `seaborn`
- `scikit-learn`, `prophet`, `numpy`

---

### 📁 Format Dataset

Wajib mengandung kolom:

| Kolom            | Tipe Data     | Contoh               |
|------------------|---------------|----------------------|
| `timestamp`      | datetime      | `2024-06-01 10:00:00`|
| `power_usage_watt` | float        | `120.5`              |

---

### 📌 Catatan

- Forecasting dilakukan per hari, bukan per jam
- Clustering mendeteksi pola konsumsi perangkat per **jam** dalam sehari
- App ini dikembangkan untuk submission **SheHacks x IDCamp 2024**

---

### 🧑‍💻 Developer

Made with ❤️ by **Rahadian Ivan**  
🚀 Submission for SheHacks x IDCamp 2024  
🔗 [Streamlit App](https://leastric-usage.streamlit.app/)  
🔗 [GitHub Repo](https://github.com/rahadianivan09/leastric)
