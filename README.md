# Analisis Biaya Asuransi Kesehatan

## Project Overview
Biaya asuransi kesehatan dapat berbeda-beda pada setiap individu. Perbedaan ini dapat dipengaruhi oleh berbagai faktor seperti usia, kondisi kesehatan, dan gaya hidup.

Proyek ini bertujuan untuk menganalisis bagaimana **usia (age)** dan **Body Mass Index (BMI)** memengaruhi **biaya asuransi kesehatan (charges)**. Selain itu, analisis juga melihat peran faktor lain seperti **status merokok, wilayah tempat tinggal, dan jumlah anak**.

Melalui analisis ini diharapkan dapat diketahui faktor apa saja yang paling berpengaruh terhadap peningkatan biaya asuransi.

---

## Business Questions

Beberapa pertanyaan yang ingin dijawab dalam proyek ini adalah:

1. Bagaimana pengaruh **usia** terhadap besarnya biaya asuransi kesehatan?
2. Bagaimana pengaruh **BMI** terhadap biaya asuransi kesehatan?
3. Apakah **status merokok** memperkuat pengaruh usia dan BMI terhadap biaya asuransi?
4. Apakah terdapat perbedaan biaya asuransi antar **wilayah (region)**, khususnya pada wilayah Southeast?
5. Apakah **jumlah anak** memiliki pengaruh terhadap biaya asuransi?

---

## Dataset

Dataset yang digunakan adalah **Medical Insurance Cost Dataset** yang berisi informasi mengenai karakteristik individu dan biaya asuransi kesehatan.

### Variabel dalam Dataset

| Variabel | Deskripsi |
|--------|-------------|
| age | Usia pemegang asuransi |
| sex | Jenis kelamin |
| bmi | Body Mass Index |
| children | Jumlah anak atau tanggungan |
| smoker | Status merokok |
| region | Wilayah tempat tinggal |
| charges | Total biaya asuransi kesehatan |

Dataset ini terdiri dari **1.338 data** dengan **7 variabel**.

---

## Data Preparation

### Data Cleaning
Beberapa tahap pembersihan data yang dilakukan:

- Mengecek **data duplikat**
- Menghapus **duplikat full row**
- Memastikan tidak ada **missing value**
- **Outlier tidak dihapus** karena nilai yang sangat tinggi masih mungkin terjadi pada biaya asuransi kesehatan.

### Data Transformation

Untuk mempermudah analisis, beberapa pengelompokan data dibuat.

#### Kategori BMI
BMI dibagi menjadi beberapa kategori:

- Underweight (<18.5)
- Normal (18.5 – 24.9)
- Overweight (25 – 29.9)
- Obese (≥30)

#### Kelompok Usia
Usia juga dikelompokkan ke dalam beberapa rentang untuk melihat pola biaya pada setiap kelompok usia.

---

## Data Analysis

Analisis dilakukan dengan melihat hubungan antara beberapa variabel, seperti:

- **Usia dan biaya asuransi**
- **BMI dan biaya asuransi**
- **Kategori BMI dan biaya asuransi**
- **Status merokok dan biaya asuransi**
- **Wilayah dan biaya asuransi**

Perbandingan dilakukan menggunakan **nilai rata-rata (average)** agar lebih mudah melihat perbedaan antar kelompok.

---

## Insight

### 1. Pengaruh Usia
Biaya asuransi cenderung meningkat seiring bertambahnya usia.  
Kelompok usia **50 tahun ke atas** memiliki rata-rata biaya asuransi paling tinggi dibandingkan kelompok usia yang lebih muda.

### 2. Pengaruh BMI
Individu dengan **BMI kategori obese** memiliki rata-rata biaya asuransi paling tinggi dibandingkan kategori BMI lainnya.

Hal ini kemungkinan karena obesitas berkaitan dengan berbagai risiko penyakit seperti **diabetes, hipertensi, dan penyakit jantung**.

### 3. Pengaruh Merokok
Individu yang **obese dan merokok** memiliki biaya asuransi jauh lebih tinggi dibandingkan individu obese yang tidak merokok.

Hal ini menunjukkan bahwa merokok dapat meningkatkan risiko kesehatan secara signifikan.

### 4. Perbedaan Wilayah
Wilayah **Southeast** memiliki rata-rata biaya asuransi yang lebih tinggi dibandingkan wilayah lain.

Namun setelah dianalisis lebih lanjut, hal ini kemungkinan dipengaruhi oleh **proporsi individu dengan BMI tinggi yang lebih besar di wilayah tersebut**, bukan semata-mata karena faktor lokasi.

### 5. Jumlah Anak
Jumlah anak tidak menunjukkan hubungan yang konsisten dengan biaya asuransi.

Hal ini menunjukkan bahwa **faktor kesehatan lebih berpengaruh** dibandingkan faktor demografis keluarga.

---

## Recommendation

### Untuk Perusahaan Asuransi
Perusahaan asuransi dapat menggunakan **usia, BMI, dan status merokok** sebagai faktor utama dalam menentukan premi asuransi karena ketiganya memiliki pengaruh yang cukup signifikan terhadap biaya asuransi.

### Strategi Pencegahan
Mendorong masyarakat untuk:

- menjaga **berat badan yang sehat**
- **mengurangi atau berhenti merokok**

Hal ini dapat membantu menurunkan risiko penyakit dan biaya kesehatan di masa depan.

### Analisis Selanjutnya
Untuk meningkatkan akurasi analisis risiko kesehatan, penelitian selanjutnya dapat menambahkan variabel lain seperti:

- aktivitas fisik
- riwayat penyakit
- pola hidup atau gaya hidup

---

## Tools yang Digunakan

- **Power BI** – Visualisasi data dan pembuatan dashboard
- **Python** – Pengolahan dan eksplorasi data

# 📊 Project Presentation

Slide presentasi lengkap dari project ini dapat dilihat pada link berikut:

🔗 [View Presentation]([https://www.canva.com/design/DAHAov_DyOg/AoL9JnlyYCqCWEZKTOsDSA/edit?utm_content=DAHAov_DyOg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton])
