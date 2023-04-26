
# Submission 2: Airline Passenger Satisfaction

Nama: Nur Muhammad Himawan

Username Dicoding: [mawann](https://www.dicoding.com/users/mawann/)

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Airline Passenger Satisfaction](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction) |
| Masalah | Pesawat merupakan pilihan transportasi yang banyak diminati karena kenyamanan dan keamanannya. Persaingan di industri penerbangan sipil saat ini semakin ketat, sehingga berbagai fitur dan layanan diberikan untuk memuaskan para pelanggannya. Maskapai perlu mengetahui kepuasaan pelanggan dari para penumpang pesawatnya, karena kepuasan pelanggan menjadi faktor penentu kinerja bisnis dan keunggulan kompetitif suatu perusahaan maskapai. |
| Solusi machine learning | Oleh karena itu, dibutuhkan solusi machine learning untuk memprediksi kepuasan penumpang dan mengidentifikasi faktor utama yang mempengaruhinya dapat membantu maskapai penerbangan dalam meningkatkan layanannya guna meraih keuntungan dalam situasi yang sulit di persaingan yang ketat saat ini. Hal ini penting untuk meningkatkan pertumbuhan dan reputasi perusahaan maskapai di masa depan. |
| Metode pengolahan | Ada beberapa metode yang digunakan dalam pengolahan data di proyek ini, melakukan data cleaning dengan menghapus beberapa fitur yang tidak dibutuhkan serta menghilangkan missing values. Kemudian, membagi dataset menjadi data training dan evaluation. Selanjutnya melakukan data validation dan transformasi fitur pada data input, baik untuk data numerikal dan categorical agar bisa digunakan pada pipeline selanjutnya. |
| Arsitektur model | Dalam proyek ini, arsitektur model yang digunakan adalah Neural Network, algoritma yang terdiri dari beberapa layer neuron yang terhubung satu sama lain. Setiap layer neuron menerima input dari layer sebelumnya dan mengeluarkan output ke layer berikutnya. Terdapat beberapa hidden layer yang masing-masing memiliki jumlah neuron yang ditentukan melalui hyperparameter tuning. Hidden layer dihubungkan satu sama lain melalui serangkaian bobot atau parameter yang diperbarui selama pelatihan. Untuk mengurangi overfitting, pada setiap hidden layer diaplikasikan dropout dengan dropout rate yang juga ditentukan melalui hyperparameter tuning. Dropout memilih beberapa neuron secara acak dari hidden layer dan mematikan fungsinya selama pelatihan. Neural Network dirasa tepat untuk digunakan dalam case ini, untuk memprediksi kepuasan penumpang maskapai penerbangan. |
| Metrik evaluasi | Metrik yang digunakan untuk mengevaluasi performa model adalah AUC (Area Under the ROC Curve), Precision, Recall, TFMA Example Count, True Positive, True Negatives, False Positive, False Negatives, dan Binary Accuracy. |
| Performa model | Performa model yang telah dibuat lumayan baik dan model sudah bisa digunakan untuk memprediksi kepuasan penumpang pesawat. Namun, perlu ditingkatkan lagi karena penulis melihat bahwa saat pelatihan, model masih terlihat overfitting walaupun sudah menerapkan hyperparameter tuning. Kemungkinan, karena data yang terlalu sedikit atau tidak representatif. |
| Opsi deployment | Proyek machine learning ini dideploy menggunakan salah satu Platform as a Service, yaitu Railway App yang dapat digunakan secara gratis. |
| Web app | Akses model serving melalui [airline-passenger-satisfaction-model](https://airline-passenger-satisfaction.up.railway.app/v1/models/airline-passenger-satisfaction-model/metadata).|
| Monitoring | Monitoring model dilakukan dengan memanfaatkan Prometheus, dan model sudah dapat digunakan dengan baik untuk memprediksi kepuasaan penumpang pesawat. Prometheus memantau dan mengumpulkan metrik dari model. Pengumpulan metrik seperti waktu respons model dan kesesuaian hasil prediksi dengan data yang sebenarnya. Hal ini dapat membantu Anda mengidentifikasi apakah model masih bekerja dengan baik atau tidak.|
| Referensi | <ul><li> Wulandari, R. & Fadlilah, R. (2019) Analisis kepuasan penumpang pesawat dengan metode Importance-Performance Analysis (IPA) di Bandara Soekarno-Hatta. Jurnal Transportasi, 19(1), 33-43.</li><li> Nurlatifah, R. & Hidayat, T. (2019) Analisis faktor-faktor yang mempengaruhi kepuasan pelanggan maskapai penerbangan di Indonesia. Jurnal Manajemen Transportasi & Logistik, 6(1), 57-67. </li></ul>|