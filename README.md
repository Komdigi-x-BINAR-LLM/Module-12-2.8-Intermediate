# Module-12-2.8-Intermediate
Teknik Evaluasi untuk Aplikasi Berbasiskan LLM

# Hands-on Komdigi: Modul 2.8 - Automated Evaluation dengan RAGAS

Selamat datang di *repository hands-on* terakhir untuk Program Intermediate!

**Tujuan:**
Di modul ini, kita beralih peran dari "Pembuat Model" menjadi "Auditor Model". Notebook ini (`Modul_2_8_RAGAS_Evaluation.ipynb`) dirancang untuk mempraktikkan evaluasi otomatis sistem RAG menggunakan framework **RAGAS** dan **OpenAI**.

**Materi Praktik:**
1.  **Setup Dataset Evaluasi (2.8.3):** Membuat dataset standar yang berisi `question`, `answer`, `contexts`, dan `ground_truth`.
2.  **RAG Metrics (2.8.6):** Menjalankan evaluasi untuk metrik **Faithfulness** (Deteksi Halusinasi) dan **Answer Relevancy**.
3.  **Analisis Hasil:** Mengubah skor mentah menjadi *Pandas DataFrame* untuk memudahkan pelaporan dan analisis *gap*.

**Prasyarat:**
* Akun Google Colab.
* **API Key OpenAI** (Wajib, karena RAGAS menggunakan GPT-3.5/4 sebagai Juri).
    * *Catatan: Jika tidak memiliki API Key, notebook menyediakan data dummy hasil evaluasi agar Anda tetap bisa belajar cara menganalisis laporannya.*

---

## Cara Menjalankan Notebook

Klik *badge* di bawah untuk membuka *notebook* langsung di Google Colab.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18kI6pGQ2ZziNozzJupygPXIqqyYtFb2C?usp=sharing)

**Hasil yang Diharapkan:**
Anda akan mendapatkan tabel laporan yang menunjukkan skor kualitas untuk setiap pertanyaan, dan secara otomatis mendeteksi mana jawaban yang "Berhalusinasi" (Faithfulness rendah) dan mana yang "Melenceng" (Relevance rendah).

Selamat mengaudit AI Anda!
