# Çiçek Görüntü Sınıflandırma (MobileNetV2)

Kaggle [Flowers](https://www.kaggle.com/datasets/l3llff/flowers) veri setinde **16 çiçek sınıfını** ayıran bir **transfer learning** + **fine-tuning** projesi.

## Öne çıkanlar

| Madde | Detay |
|------|--------|
| Model | MobileNetV2 (ImageNet pretrained) |
| Input size | 160×160 |
| Sınıf sayısı | 16 |
| Pipeline | Stage-1 head training → Stage-2 fine-tune (son 20 katman) |
| Metrikler | Accuracy, Precision, Recall, F1, confusion matrix |

## Sonuçlar (test set)

| Metrik | Skor |
|--------|------:|
| Accuracy | **91.52%** |
| Precision (macro) | 91.59% |
| Recall (macro) | 91.61% |
| F1-Score (macro) | **91.40%** |

## Kullanılan teknolojiler

- Python, TensorFlow / Keras
- scikit-learn (metrikler)
- Matplotlib / Seaborn (grafikler)
- kagglehub (veri seti indirme)
- Google Colab (T4 GPU önerilir)

## Nasıl çalıştırılır?

1. [`sinir_final.ipynb`](sinir_final.ipynb) dosyasını [Google Colab](https://colab.research.google.com) veya Jupyter’da aç.
2. Runtime → Change runtime type → **GPU**.
3. Hücreleri yukarıdan aşağı sırayla çalıştır.

```bash
pip install -r requirements.txt
```

Veri seti notebook içinde Kaggle üzerinden indirilir. Büyük veri dosyaları bu repoda tutulmaz.

## Proje yapısı

```text
sinir-agi/
├── README.md
├── requirements.txt
├── .gitignore
└── sinir_final.ipynb
```

## Lisans

Eğitim / portfolio amaçlı proje. Veri seti lisansı Kaggle kaynak sayfasındaki koşullara tabidir.
