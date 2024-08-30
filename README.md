# Capstone-3

### Permasalahan

Risiko yang harus diperhitungkan oleh setiap perusahaan asuransi adalah risiko klaim dari nasabah. Klaim asuransi terjadi ketika seorang pemegang polis mengalami kerugian atau kejadian yang dicakup oleh polis asuransi mereka dan meminta perusahaan asuransi untuk memberikan kompensasi sesuai dengan ketentuan yang tercantum dalam polis.

Dalam asuransi perjalanan, kerugian yang dicover biasanya meliputi biaya medis darurat, yang mencakup perawatan rumah sakit dan obat-obatan jika pelancong jatuh sakit atau terluka. Selain itu, asuransi ini juga mencakup kompensasi untuk pembatalan perjalanan yang disebabkan oleh alasan yang dijamin, seperti sakit mendadak atau kejadian darurat. Kerugian lainnya yang dicover termasuk kehilangan atau kerusakan bagasi, keterlambatan perjalanan yang mengakibatkan biaya tambahan, serta evakuasi medis darurat jika diperlukan. Beberapa polis juga menyediakan perlindungan untuk kehilangan dokumen penting, seperti paspor, yang sangat penting untuk memastikan perjalanan tetap lancar dan aman.

Perusahaan asuransi dapat mengalami kerugian apabila tidak memitigasi risiko klaim dengan baik. Kerugian terjadi ketika pengeluaran perusahaan akibat klaim lebih besar dari pendapatan dari biaya polis asuransi yang diterima. Oleh karena itu penting bagi sebuah perusahaan untuk memitigasi risiko klaim, dan perusahaan juga dapat menentukan harga polis berdasarkan 

Oleh karena itu untuk memitigasi risiko klaim pada asuransi perjalanan dibuatlah pemodelan dengan pendekatan *machine learning*

### Pemodelan
Metode yang dicoba dalam pemodelan ini antara lain adalah Logistic Regression, KNN, DT, Hard Voting, Soft Voting, Stacking, RF, Adaboost, Gradboost, dan Xgboost.

### Hasil
Model terbaik berdasarkan besarnya net income adalah model XGB Classifier dengan menggunakan random oversampler, winsorizer, dan tanpa scaler. Pada pemodelan rare label dikelompokan menjadi satu grup yang nantinya setiap variabel kategori di encode dengan one hot encoder. Pada model ini didapatkan threshold terbaik sebesar 65% dalam memaksimalkan net income. Apabila perusahaan asuransi perjalanan memfilter orang dengan probabilitas klaim diatas 65%, terjadi **peningkatan net income sebesar 66,61%** dari 4.567 milyar menjadi 7.609 milyar rupiah dengan net income per polis sebesar 959.213 ribu rupiah.
