# Final Submission: Machine Learning Operations(MLops) Pipeline - Klasifikasi Penyakit Stroke
Nama: Novan Nur Hidayat

Username dicoding: fannof

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Brain Stroke Dataset](https://www.kaggle.com/datasets/jillanisofttech/brain-stroke-dataset) | 
| Masalah | Stroke adalah penyakit dengan kondisi ketika pasokan darah ke otak terganggu karena penyumbatan di dalam otak (stroke iskemik) atau pecahnya pembuluh darah (stroke hemoragik). Kondisi tersebut menyebabkan area tertentu pada otak tidak mendapat suplai oksigen dan nutrisi yang cukup sehingga terjadi kematian sel-sel pada otak. |
| Solusi machine learning | Untuk mempermudah pengecekan apakah seseorang mengalami penyakit stroke atau tidak dengan membuat model machine learning dimana ia akan memprediksi secara otomatis apakah orang tersebut teridetifikasi penyakit stroke atau tidaknya sesuai ciri-ciri yang akan disebutkan oleh pasien. |
| Metode pengolahan | Deskripsi metode pengolahan data yang digunakan |
| Arsitektur model | Model merupakan model jaringan saraf tiruan (neural network) yang digunakan untuk prediksi dengan input layer berupa fitur numerik dan kategorik. Model memiliki beberapa dense (fully connected) layer dengan aktivasi ReLU (Rectified Linear Unit) dan hidden layer dengan lapisan 256, 64, 16 neuron. Output layer hanya memiliki 1 neuron dengan aktivasi sigmoid, karena ini adalah tugas binary classification (klasifikasi biner). Aktivasi sigmoid akan mengeluarkan nilai antara 0 dan 1 yang kemudian dapat diinterpretasikan sebagai probabilitas kelas. Model dikompilasi dengan optimizer Adam, yang merupakan algoritma optimisasi yang efisien dan sering digunakan dalam pelatihan neural network. loss="binary_crossentropy" digunakan karena ini adalah masalah klasifikasi biner. |
| Metrik evaluasi | Metrik yang digunakan untuk mengevaluasi model adalah BinaryAccuracy, yang mengukur seberapa sering prediksi model benar berdasarkan ambang batas 0.5 (untuk klasifikasi biner). Training loss berada di angka 0.0139 dan binary_accuracy di angka 0.9941. Hal ini menunjukkan bahwa model memiliki akurasi yang sangat tinggi (99.41%) di data training, dengan loss yang sangat rendah, ini artinya model bisa mempelajari pola dari data training dengan sangat baik. Validation loss berada di angka 2.3555 dan val_binary_accuracy di angka 0.9172, meskipun loss pada data validasi relatif lebih tinggi, akurasi validasi sebesar 91.72% menunjukkan bahwa model mampu menggeneralisasi dengan baik pada data yang belum pernah dilihat sebelumnya. |
| Performa model | Secara keseluruhan, hasil ini menunjukkan bahwa model sudah cukup baik dalam melakukan prediksi, meskipun perbedaan antara training dan validation loss menunjukkan potensi adanya overfitting yang ringan. Namun, dengan akurasi validasi yang tinggi, performa model sudah berada di tingkat yang memadai. |
| Opsi deployment | Deksripsi tentang opsi deployment |
| Web app | Tautan web app yang digunakan untuk mengakses model serving. Contoh: [nama-model](https://model-resiko-kredit.herokuapp.com/v1/models/model-resiko-kredit/metadata)|
| Monitoring | Deksripsi terkait hasil monitoring dari model serving |
