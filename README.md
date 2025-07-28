#  Waifu Matcher AI
Aplikasi real-time face recognition yang mencocokkan wajahmu dengan karakter waifu dari berbagai anime menggunakan model deep learning (CNN).
Dilengkapi dengan skor confidence dan alasan personal mengapa karakter tersebut cocok denganmu secara visual dan kepribadian.


# Fitur Utama
-Deteksi wajah real-time dari webcam
-Pencocokan wajah ke karakter waifu dari lebih dari 100+ karakter anime
-Skor kuantitatif (confidence) sebagai dasar ilmiah kecocokan
-Penjelasan alasan cocok dengan waifu secara personal
-Tampilan UI elegan, tema dark/light, dan responsif
-Disertai source code lengkap dan mudah dijalankan

# Penjelasan Ilmiah
1.Dasar Kecocokan Wajah
Sistem menggunakan Convolutional Neural Network (CNN) untuk mengekstrak embedding wajah. Embedding ini merepresentasikan struktur wajah seperti:

*bentuk mata, hidung, dan bibir
*kontur wajah
*rasio dimensi wajah
Model kemudian menghitung kemiripan embedding user dengan dataset waifu, lalu mengembalikan karakter dengan skor tertinggi (confidence score).

2.Dasar Kuantitatif
Nilai confidence (%) menunjukkan seberapa mirip wajah pengguna dengan karakter tertentu secara numerik berdasarkan hasil softmax prediksi model.
Contoh output:
{"match": "asuna_(sao)", "confidence": "92.38%", "reason": "Kamu punya aura pemimpin yang lembut dan setia, cocok banget sama Asuna."}


# Teknologi yang Digunakan
-----------------------------------------------------------------
| Teknologi           | Deskripsi                               |
| ------------------- | --------------------------------------- |
| Python & Flask      | Web framework backend                   |
| OpenCV              | Deteksi wajah real-time                 |
| TensorFlow / Keras  | Model deep learning untuk face matching |
| HTML + CSS + JS     | Frontend responsif                      |
| Font Awesome        | Ikon dan antarmuka modern               |
| SpeechSynthesis API | Text-to-speech langsung di browser      |
-----------------------------------------------------------------

# Struktur Proyek 
waifu-matcher-ai/
├── app.py
├── templates/
│   └── index.html
├── static/
│   └── unknown_faces/
├── model/
│   ├── face_recognition_model.h5
│   ├── waifu_match_model.h5
│   ├── label_encoder_classes.npy
│   └── waifu_label_encoder_classes.npy
├── waifu_reasons.py
└── README.md

# Pengembang
Rais Rasyad Shidiq – @Reyeis

