# Certainty-Factor-Fuzzy-Logic
# TASLIM NURALIM 2306032
## 📌 Deskripsi

Proyek ini mencakup dua pendekatan untuk pengambilan keputusan:
- **Certainty Factor (CF)** untuk diagnosa penyakit berdasarkan gejala.
- **Fuzzy Logic** untuk kontrol kecepatan kipas berdasarkan suhu dan kelembaban.
---

## 🧠 Certainty Factor (CF)

### Fungsi:
```python
def hitung_cf(gejala_user, pengetahuan_pakar):
    ...
```

### Studi Kasus:
- Diagnosa `flu`, `rheumatoid_arthritis`, dan `diabetes` berdasarkan gejala dengan CF.
- Pengaruh bobot gejala pada hasil diagnosis (terutama `penurunan_berat_badan`, dll).

### Eksperimen:
- Mengubah nilai CF `"demam"` dari `0.7` ke `0.2`.
- Menambahkan 5 gejala baru dan melihat perubahan diagnosis.

---

## 🌡️ Fuzzy Logic

### Variabel:
- `temperature`: dingin, normal, panas
- `humidity`: kering, normal, lembab
- `fan_speed`: mati, rendah, sedang, tinggi, maksimal

### Rules:
```python
Rule(temperature['panas'] & humidity['lembab'], fan_speed['maksimal'])
```

### Eksperimen:
- Input suhu 22°C: perhatikan perubahan nilai keanggotaan fuzzy.
- Tambahkan variabel kelembaban dan lihat perubahan kecepatan kipas.

---

## 🧪 Cara Menjalankan

1. Jalankan kode Certainty Factor (Python Script).
2. Jalankan notebook / script untuk Fuzzy Logic.
3. Amati output pada terminal / Jupyter Notebook.
4. Ubah parameter dan bandingkan hasil diagnosis atau output kontrol.

---

## 🗂 Struktur File
```
├── cf_diagnosis.py
├── fuzzy_suhu.py
├── fuzzy_ac_control.py
└── README.md
```

---

## 👨‍🎓 Catatan Tambahan

- Certainty Factor cocok untuk diagnosis berbasis aturan.
- Fuzzy Logic cocok untuk sistem kontrol yang fleksibel.
- Gunakan visualisasi untuk memahami perubahan nilai derajat keanggotaan fuzzy.

---
