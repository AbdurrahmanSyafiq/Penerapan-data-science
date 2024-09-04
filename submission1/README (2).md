# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

Username : assegafsyafiq1@gmail.com
Password : root123

## Business Understanding

Jaya Jaya Maju merupakan salah satu perusahaan multinasional yang telah berdiri sejak tahun 2000. Ia memiliki lebih dari 1000 karyawan yang tersebar di seluruh penjuru negeri.
Walaupun telah menjadi menjadi perusahaan yang cukup besar, Jaya Jaya Maju masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%.

### Permasalahan Bisnis

Dari Permasalahan yang dimiliki yaitu tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan keseluruhan) hingga lebih dari 10%. Terdapat beberapa faktor:

- Kenaikan gaji yang tidak terlalu besar (SalaryHike) pada karyawan yang keluar
- Kurang mengapresiasai kinerja karyawan

### Cakupan Proyek

Proyek ini bertujuan untuk menganalisis data karyawan di perusahaan Jaya Jaya Maju, dengan fokus pada faktor-faktor yang mempengaruhi tingkat attrition (keluar/mengundurkan diri) karyawan. Dalam proyek ini, saya mengerjakan beberapa tugas utama:

1. Analisis data karyawan
   - Mengumpulkan dan membersihkan data karyawan untuk memastikan kualitas data yang digunakan.
   - Melakukan eksplorasi data untuk mengidentifikasi tren dan pola yang signifikan terkait dengan faktor-faktor seperti tingkat kenaikan gaji (SalaryHike), keterlibatan kerja (Job Involvement), overtime, tingkat job level, dan MonthlyIncome.
2. Pembuatan Dashboard
   - Mendesain dan membangun dashboard interaktif yang memungkinkan tim manajemen untuk memantau indikator utama terkait attrition.
   - Menyajikan visualisasi data dalam bentuk bar chart, untuk menggambarkan hubungan antara faktor-faktor yang dianalisis dengan tingkat attrition.
   - Dashboard ini memungkinkan pemantauan yang mudah dan cepat terhadap karyawan yang berisiko tinggi untuk meninggalkan perusahaan, serta membantu dalam pengambilan keputusan yang lebih baik.

### Persiapan

Sumber data: https://github.com/dicodingacademy/dicoding_dataset/blob/main/employee/employee_data.csv
Setup environment:

```
pandas==2.0.3
numpy==1.25.2
matplotlib==3.7.2
seaborn==0.12.2
Install Docker
https://docs.docker.com/desktop/install/windows-install/
Pull Metabase Image From Docker
docker pull metabase/metabase:v0.46.4
Run Docker on localhost:3000
docker run -p 3000:3000 --name metabase metabase/metabase

```

## Business Dashboard

Dalam bussines dashboard yang telah dibuat, telah saya visualisasikan analisis terhadap :

1. Analisis attrition pada monthlyIncome
2. Analisis jumlah karyawan berdasarkan salaryHike
3. Analisis jumlah karyawan berdasarkan salaryHike dan OverTime
4. Analisis jumlah karyawan berdasarkan jobInvolvement dan SalaryHike
5. Analisis jumlah karyawan berdasarkan SalaryHike dan PerformanceRating
6. Analisis jumlah karyawan berdasarkan job level dan salaryHike

## Conclusion

Dari analisis yang telah dilakukan, terdapat 5 feature penting yang menyebabkan karyawan memutuskan untuk keluar dari perusahaan.
5 Feature itu adalah monthlyIncome, salaryHike, OverTime, JobInvolvement, JobLevel, dan PerformanceRating.

1. Analisis attrition pada monthlyIncome
   Pada analisis yang telah dilakukan, rata-rata monthlyIncome yang didapatkan oleh karyawan yang keluar lebih kecil daripada karyawan yang stay
2. Analisis jumlah karyawan berdasarkan salaryHike
   Pada analisis yang telah dilakukan, mayoritas kenaikan gaji yang diterima oleh karyawan yang keluar berada pada tingkat low (11-15%)
3. Analisis jumlah karyawan berdasarkan salaryHike dan OverTime
   Pada analisis yang telah dilakukan, bahkan karyawan dengan kenaikan gaji berada pada tingkat low juga mendapatkan overtime dengan perbandingan 61 overtime dan 51 tidak overtime.
4. Analisis jumlah karyawan berdasarkan jobInvolvement dan SalaryHike
   Pada analisis yang telah dilakukan, mayoritas karyawan yang keluar berada pada tingkat 3(Excelent) atau 4(Outstanding) namun hal itu tidak sebanding dengan kenaikan gaji yang mereka dapat
5. Analisis jumlah karyawan berdasarkan SalaryHike dan PerformanceRating
   Pada analisis yang telah dilakukan, kenaikan gaji yang kecil berbanding lurus dengan performanceRating yang lebih rendah.
6. Analisis jumlah karyawan berdasarkan job level dan salaryHike
   Pada Job level yang rendah, kenaikan gaji tidak sebanding dengan karyawan yang memiliki job level yang tinggi.

Perusahaan perlu untuk segera memperhatikan 6 Analisa tersebut jika ingin menahan tingkat attrition rate pada perusahaan
Jelaskan konklusi dari proyek yang dikerjakan.

### Rekomendasi Action Items (Optional)

Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

## **Dari analisis yang dilakukan hal ini adalah beberapa alasan yang membuat rasio jumlah karyawan yang keluar lebih dari 10% :**

1. Kenaikan gaji yang tidak terlalu besar (SalaryHike) pada karyawan yang keluar
   Solusi : Pihak Jaya Jaya Maju sebaiknya mempertimbangkan kenaikan gaji yang sesuai pada semua karyawan yang terlibat. Kenaikan gaji yang rendah tersebut juga mempengaruhi performance rating yang didominasi oleh performa yang rendah pada karyawan yang keluar. Hal ini ditunjukkan pada analisis SalaryHike, analisis SalaryHike + PerformanceRating. Kenaikan gaji yang sesuai akan memotivasi karyawan dalam berkerja. Selain kenaikan gaji, pertimbangkan untuk menerapkan program bonus tahunan yang berdasarkan pencapaian kinerja individu maupun tim yang dapat menjadi motivator tambahan bagi karyawan untuk mencapai target kinerja yang lebih tinggi.
2. Kurang mengapresiasai kinerja karyawan
   Job Involvement pada karyawan yang keluar didominasi pada tingkat 3(Excelent) dan 4(Outstanding) menanadakan karyawan cenderung lebih termotivasi, merasa memiliki tanggung jawab yang besar, dan lebih peduli dengan hasil dari pekerjaan mereka. Namun hal ini tidak sebanding dengan kenaikan gaji yang rendah dan banyaknya karyawan yang mendapatkan overtime. Hal ini ditunjukkan pada analisis. Hal ini ditunjukkan pada analisis JobInvolvement + SalaryHike, JobLevel + SalaryHike, SalaryHike + Overtime, dan JobLevel + SalaryHike + Overtime.
   **Solusi yang Dapat Dipertimbangkan:**

- Evaluasi dan Revisi Kebijakan Kenaikan Gaji:
  Kenaikan Gaji yang Lebih Adil:
  Perusahaan harus mempertimbangkan untuk menyesuaikan kebijakan kenaikan gaji, terutama bagi karyawan dengan job involvement tinggi. Karyawan yang menunjukkan komitmen dan kinerja luar biasa harus mendapatkan kenaikan gaji yang sepadan.
  Kenaikan Gaji Berdasarkan Kinerja:
  Implementasi sistem kenaikan gaji berbasis kinerja yang jelas dan transparan bisa menjadi solusi. Karyawan harus tahu bahwa kontribusi mereka dihargai dan diakui secara finansial.
  Pengelolaan Overtime yang Lebih Baik:

- Pengurangan Overtime:
  Mengurangi jumlah overtime bisa meningkatkan kepuasan kerja dan keseimbangan kehidupan kerja karyawan. Overtime yang berlebihan bisa menjadi tanda bahwa beban kerja tidak didistribusikan dengan baik, dan ini harus dievaluasi.
  Kompensasi untuk Overtime:
  Jika overtime tidak dapat dihindari, pastikan bahwa karyawan mendapatkan kompensasi yang sesuai, baik dalam bentuk pembayaran tambahan atau waktu cuti yang setara.
