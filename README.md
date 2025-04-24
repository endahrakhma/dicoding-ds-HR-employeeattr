# Submission Pertama : Menyelesaikan Permasalahan Human Resources
## Case Understanding
Analisa attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) sangat penting bagi perusahaan karena memberikan gambaran yang jelas tentang kesehatan organisasi, kepuasan karyawan, dan efektivitas manajemen sumber daya manusia. Hal ini membantu HR untuk lebih tepat sasaran dalam mengintervensi area yang bermasalah.
## Latar Belakang
Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000. Ia memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri. Walaupun telah menjadi menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate hingga lebih dari 10%.
## Permasalahan
Untuk mencegah attrition rate semakin tinggi, maka diperlukan identifikasi berbagai faktor yang mempengaruhi tingginya attrition rate tersebut.
## Cakupan Proyek
Setelah pendefinisian masalah, kita kumpulkan data yang diperlukan dan mempelajari/memahaminya sehingga dapat memformulasikan masalah menjadi bentuk ML task, dalam kasus ini adalah klasifikasi. Model terbaik yaitu dengan akurasi yang optimal diperoleh setelah data preprocessing sampai optimasi model dapat diimplementasikan untuk prediksi attrition yang nantinya keluar sebagai report. Report inilah yang dimanfaatkan untuk membangun dashboard dengan visualisasi data yang menarik sehingga dapat mengetahui dengan mudah faktor-faktor yang mempengaruhi attrition rate Jaya Jaya Maju.
    
## Persiapan
[Sumber Data](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee)

ML tasks:

    a. Data Collection dan Data Understanding
    b. Exploratory Data Analysis (EDA) : analisa statistik dan visualisasi
    c. Data Preprocessing : Feature Engineering, encoding, outlier handling, feature scaling
    d. Modeling : splitting data, over sampling dengan SMOTE, model selection (memilih algoritma ML classifier yang tepat)
    e. Evaluasi : confussion matrix (accuracy)
    f. Optimasi model : hyperparameter tuning, gridSearchCV
    g. Feature Importance : menentukan top 10 fitur penting dalam model 
    h. Membuat pipeline model yang digunakan
    h. Penyimpanan model : format .pkl
    i. Implementasi model : prediksi attrition
    j. Penyimpanan dataset hasil prediksi : reporting dan visualisasi dashboard

## HR Dashboard

  HR Dashboard ini dibuat menggunakan [Looker Studio](https://lookerstudio.google.com/reporting/93891af4-4da9-4e63-b390-df9be315ee24).

#### Kesimpulan
    a. Top 10 fitur penting yang mempengaruhi model antara lain OverTime, TotalWorkingYears, MonthlyIncome, JobSatisfaction, EnvironmentSatisfaction, Age, JobLevel, YearsAtCompany, MaritalStatus, StockOptionLevel yang mana akan kita fokuskan pada visualisasi dalam dashboard.
    b. Attrition rate sebesar 12,6% atau sebanyak 185 orang, didominasi oleh:
        - pria, single
        - usia 31-35 tahun
        - berpengalaman kerja 5+
        - lama bekerja di perusahaan 2-4 tahun
        - job roles : laboratory technician
        - job level : 1
        - pendapatan per bulan : 1000-5000
        - nilai kepuasan pada pekerjaan : 3
        - nilai kepuasan pada lingkungan kerja : 1
        - stock option level : 0
    c. Secara umum, sebagian besar karyawan:
        - memiliki performa kerja yang baik dengan nilai 3, dikarenakan sudah berpengalaman kerja selama 5+ tahun
        - berdedikasi tinggi pada pekerjaan, mereka puas pada pekerjaan yang dijalankan dan beberapa karyawan pada setiap job roles bekerja overtime
        - bekerja di perusahaan selama 2-4 tahun
        - Stock Option Level 0, tidak diberikan atau diberikan jumlah minimum/insignifikan dari opsi saham oleh perusahaan, dikarenakan belum eligible atau mungkin statusnya kontrak bukan full-time.
        
#### Rekomendasi Aksi

1. Ciptakan onboarding yang kuat dan budaya kerja yang positif, terbuka, dan kolaboratif sehingga karyawan merasa diterima, siap kerja dan nyaman bekerja.
2. Sediakan ruang bagi karyawan untuk memberi masukan (survey, feedback rutin)
3. 1 job level memiliki monthly income yang bervariasi, maka sediakan jalur karier (career path) dan promosi berbasis kinerja yang jelas.
4. Adanya fenomena overtime, pastikan beban kerja tidak berlebihan dan jam kerja wajar. 1 job level beban kerja yang merata.
5. Pastikan gaji kompetitif di industri sejenis.
6. Tambahkan insentif finasial ataupun non-finansial, seperti bonus kinerja, cuti tambahan terutama pada karyawan yang bekerja overtime.
7. Stock option adalah hak (bukan kewajiban) yang diberikan perusahaan kepada karyawannya untuk membeli saham perusahaan di harga tertentu (strike price) dalam jangka waktu tertentu. Maka perlu ditinjau ulang kebijakan terkait Stock Option Level yang diberikan kepada karyawan berdasarkan job roles, masa kerja, atau job level/tanggung jawab mereka dalam rangka memberikan insentif jangka panjang kepada karyawan agar tetap bekerja di perusahaan dan turut berkontribusi terhadap pertumbuhan perusahaan.
