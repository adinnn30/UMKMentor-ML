# UMKMentor-ML

Repository Machine Learning untuk fitur **Sentiment Analysis** pada proyek **UMKMentor**, sebuah platform yang membantu calon seller UMKM melakukan pengambilan keputusan berbasis data melalui analisis pasar, analisis sentimen ulasan pelanggan, dan simulasi profitabilitas marketplace.

## Deskripsi Proyek

Fitur Sentiment Analysis dikembangkan untuk mengklasifikasikan ulasan pelanggan ke dalam tiga kategori sentimen:

* Positif
* Netral
* Negatif

Model yang digunakan pada tahap deployment adalah **TF-IDF + Linear SVM** karena memiliki ukuran model yang lebih ringan dan lebih mudah diintegrasikan ke backend dibandingkan model transformer.

## Dataset

Dataset terdiri dari **67.200 ulasan produk** yang telah melalui proses pembersihan dan preprocessing.

Kategori yang digunakan:

* Elektronik
* Pertukangan
* Olahraga
* Hiburan
* Fashion
* Kecantikan
* Makanan dan Minuman

## Struktur Repository

```text
UMKMentor-ML
│
├── notebooks/
│   └── tfidf_svm_all_category.ipynb
│
├── models/
│   ├── svm_umkmentor_all_category.pkl
│   ├── tfidf_umkmentor_all_category.pkl
│   └── label_map.pkl
│
├── dataset/
│   └── clean_dataset_umkmentor_all_category.csv
│
├── requirements.txt
│
└── README.md
```

## Model

Algoritma yang digunakan:

* TF-IDF Vectorizer
* Linear Support Vector Machine (Linear SVM)

## Hasil Evaluasi

| Metric            | Score  |
| ----------------- | ------ |
| Accuracy          | 86.19% |
| Weighted F1-Score | 86.27% |
| Macro F1-Score    | 69.68% |

## File Model

* `svm_umkmentor_all_category.pkl`
* `tfidf_umkmentor_all_category.pkl`
* `label_map.pkl`

## Instalasi

```bash
pip install -r requirements.txt
```

## Pengembang

Tim Capstone PJK-GM006 – UMKMentor

Kontributor Sentiment Analysis:

* Adinda Intan Erlita
* Jerry Lim
