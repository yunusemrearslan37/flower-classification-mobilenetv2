# Flower Image Classification (MobileNetV2)

16-class flower image classification with **transfer learning** and **fine-tuning** on the Kaggle [Flowers](https://www.kaggle.com/datasets/l3llff/flowers) dataset.

## Highlights

| Item | Detail |
|------|--------|
| Model | MobileNetV2 (ImageNet pretrained) |
| Input size | 160×160 |
| Classes | 16 flower species |
| Pipeline | Stage-1 head training → Stage-2 fine-tune (last 20 layers) |
| Metrics | Accuracy, Precision, Recall, F1, confusion matrix |

## Results (test set)

| Metric | Score |
|--------|------:|
| Accuracy | **91.52%** |
| Precision (macro) | 91.59% |
| Recall (macro) | 91.61% |
| F1-Score (macro) | **91.40%** |

## Tech stack

- Python, TensorFlow / Keras
- scikit-learn (metrics)
- Matplotlib / Seaborn (plots)
- kagglehub (dataset download)
- Google Colab (T4 GPU recommended)

## How to run

1. Open [`sinir_final.ipynb`](sinir_final.ipynb) in [Google Colab](https://colab.research.google.com) or Jupyter.
2. Runtime → Change runtime type → **GPU**.
3. Run all cells top to bottom.

```bash
pip install -r requirements.txt
```

Dataset is fetched in the notebook via Kaggle (Colab cache / kagglehub). No large data files are stored in this repo.

## Project structure

```text
sinir-agi/
├── README.md
├── requirements.txt
├── .gitignore
└── sinir_final.ipynb
```

## License

Educational / portfolio project. Dataset license follows the Kaggle source page.
