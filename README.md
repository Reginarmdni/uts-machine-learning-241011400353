# UTS Machine Learning

**Identitas Mahasiswa**
- Nama  : Regina Ramadhani
- NIM   : 241011400353
- Kelas : 05TPLE005

---

## 📂 Isi Repositori
1. `tugas_UTS.ipynb` : Notebook Jupyter berisi pengerjaan Soal Bagian A, B, C, dan Bonus.
2. `Ads_Data.csv` : Dataset biaya iklan dan penjualan.
3. `Email_Data.csv` : Dataset fitur email dan label spam.
4. `README.md` : Dokumentasi ringkasan pengerjaan tugas UTS.

---

## 📊 Ringkasan Hasil Pengerjaan

### 1. Bagian A – Linear Regression (Ads Data)
- **Persamaan Garis Regresi**: $\hat{y} = 26.5629 + 9.3264 \times X$
- **Interpretasi**: Setiap kenaikan biaya iklan sebesar 1 juta Rp diproyeksikan meningkatkan penjualan sebesar **9.3264 juta Rp**.
- **Evaluasi Model**: Diimplementasikan manual menggunakan NumPy dengan metrik MAE, MSE, RMSE, dan $R^2$.
- **Eksperimen Gradient Descent**:
  - `LR = 0.001`: Terlalu lambat konvergen.
  - `LR = 0.02`: Pas/optimal, mendekati hasil Normal Equation.
  - `LR = 0.1`: Divergen / *exploding gradient* karena learning rate terlalu besar.

### 2. Bagian B – Logistic Regression (Email Spam)
- **Persamaan Model**: $P(\text{Spam}) = \sigma(b + m_1 \cdot \text{JumlahLink} + m_2 \cdot \text{KataPromo})$
- **Evaluasi Model**: Diimplementasikan manual menggunakan NumPy dengan metrik Accuracy, Precision, Recall, dan F1-Score.
- **Pilihan Threshold**: Dipilih **Threshold 0.7** untuk meminimalkan *False Positive* (FP) agar email penting tidak salah tersaring ke folder Spam.

### 3. Bagian C – Pemahaman Konsep
- Seluruh 5 pertanyaan konsep (alasan nama Logistic Regression, Normal Equation vs GD, Overfitting & Data Testing, MSE vs Log Loss, serta pengaruh `random_state`) telah dijawab lengkap pada notebook.

### 4. Bonus – Perbandingan dengan scikit-learn
- Perbandingan antara model buatan sendiri dan `scikit-learn` menghasilkan nilai yang identik/setara.
