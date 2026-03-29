# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri. Walaupun telah menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas pada tingginya **attrition rate** (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%.

Departemen HR membutuhkan bantuan untuk mengidentifikasi berbagai faktor yang mempengaruhi tingginya attrition rate tersebut, sekaligus membutuhkan business dashboard untuk memonitor faktor-faktor tersebut secara berkelanjutan.

### Permasalahan Bisnis

Permasalahan bisnis yang akan diselesaikan dalam proyek ini adalah:

1. Faktor-faktor apa saja yang paling berpengaruh terhadap tingginya attrition rate karyawan di perusahaan Jaya Jaya Maju?
2. Bagaimana perusahaan dapat memonitor kondisi karyawan secara real-time untuk mencegah attrition lebih lanjut?
3. Kelompok karyawan mana yang paling berisiko untuk melakukan attrition sehingga perlu mendapat perhatian lebih?

### Cakupan Proyek

Cakupan proyek yang akan dikerjakan meliputi:

1. **Data Understanding** — memahami struktur dan kualitas dataset karyawan Jaya Jaya Maju
2. **Data Preparation** — membersihkan data, menangani missing values, dan melakukan encoding
3. **Exploratory Data Analysis (EDA)** — menganalisis faktor-faktor yang berkorelasi dengan attrition
4. **Business Dashboard** — membuat dashboard interaktif menggunakan Looker Studio untuk monitoring HR

### Persiapan

Sumber data: Dataset karyawan Jaya Jaya Maju (`employee_data.csv`) yang berisi 1.470 baris dan 35 kolom, mencakup data demografi, metrik pekerjaan, dan status attrition karyawan.

Setup environment:

```bash
# Install dependencies
pip install -r requirements.txt

# Jalankan notebook
jupyter notebook notebook.ipynb
```

## Business Dashboard

Dashboard dibuat menggunakan **Looker Studio** dan dapat diakses melalui link berikut:

🔗 **Link Dashboard:** https://lookerstudio.google.com/reporting/1932d1b7-f616-4fbd-bb67-701246b6f424

Dashboard ini menampilkan:

- **KPI Utama:** Total karyawan aktif dan attrition rate keseluruhan
- **Attrition by Department:** Perbandingan tingkat attrition antar departemen
- **Attrition vs OverTime:** Pengaruh lembur terhadap keputusan karyawan untuk keluar
- **Attrition vs Monthly Income:** Hubungan antara kompensasi dan attrition
- **Attrition vs Job Satisfaction:** Dampak kepuasan kerja terhadap attrition rate

Dashboard dirancang untuk membantu manajer HR memonitor faktor-faktor risiko attrition secara visual dan mudah dipahami.

## Conclusion

Berdasarkan analisis data yang telah dilakukan terhadap dataset karyawan Jaya Jaya Maju, ditemukan beberapa faktor utama yang berkontribusi terhadap tingginya attrition rate:

1. **OverTime** — Karyawan yang sering melakukan overtime memiliki attrition rate yang jauh lebih tinggi dibandingkan yang tidak. Beban kerja berlebih menjadi salah satu pemicu utama keputusan resign.
2. **Monthly Income** — Karyawan dengan pendapatan lebih rendah cenderung lebih sering keluar dari perusahaan. Kesenjangan kompensasi menjadi faktor yang signifikan.
3. **Job Satisfaction** — Karyawan dengan tingkat kepuasan kerja rendah (level 1–2) memiliki kemungkinan resign yang lebih tinggi dibandingkan yang merasa puas.
4. **Years at Company** — Karyawan dengan masa kerja pendek (0–5 tahun) paling rentan mengalami attrition, menunjukkan bahwa fase awal karier sangat kritis untuk retensi.
5. **Department** — Departemen Sales memiliki attrition rate tertinggi dibandingkan departemen lainnya.

Secara keseluruhan, attrition rate perusahaan Jaya Jaya Maju berada di angka **~16.92%**, melebihi ambang batas 10% yang dianggap wajar. Intervensi yang tepat pada faktor-faktor di atas dapat membantu menurunkan angka ini secara signifikan.

### Rekomendasi Action Items (Optional)

Berikut beberapa rekomendasi action items yang dapat dilakukan perusahaan guna menyelesaikan permasalahan attrition:

- **Mengurangi beban overtime karyawan** — Evaluasi dan redistribusi beban kerja secara merata. Pertimbangkan penambahan tenaga kerja di divisi yang kekurangan sumber daya, terutama di departemen Sales.
- **Meningkatkan kepuasan kerja melalui program engagement** — Lakukan survei kepuasan karyawan secara berkala, sediakan jalur pengembangan karier yang jelas, dan tingkatkan komunikasi antara manajer dan tim.
- **Meninjau kembali kompensasi karyawan dengan gaji rendah** — Lakukan benchmarking gaji terhadap standar industri dan prioritaskan penyesuaian untuk karyawan dengan performa baik namun bergaji di bawah rata-rata.
- **Memperkuat program onboarding untuk karyawan baru** — Karyawan dengan masa kerja 0–5 tahun paling rentan keluar. Program mentoring dan check-in rutin di tahun pertama dapat meningkatkan retensi secara signifikan.
