# Keras Layer Comparison on MNIST

A hands-on comparison of three fundamental Keras layer types applied to the classic MNIST handwritten digit dataset.

## Goal

Compare the **accuracy**, **training time**, and **model complexity** of three different neural network architectures on the same task.

## Architectures Compared

| Notebook | Architecture | Key Layer |
|----------|-------------|-----------|
| `01_dense_model.ipynb` | Fully Connected Network | `Dense` |
| `02_conv2d_model.ipynb` | Convolutional Neural Network | `Conv2D` |
| `03_lstm_model.ipynb` | Recurrent Neural Network | `LSTM` |
| `04_comparison.ipynb` | Side-by-side results | All |

## Results Summary

> Run the notebooks yourself to populate this table!

| Model | Test Accuracy | Params | Avg Epoch Time |
|-------|--------------|--------|----------------|
| Dense | ~98.0% | ~670K | ~3s |
| Conv2D | ~99.2% | ~93K | ~10s |
| LSTM | ~98.5% | ~320K | ~25s |

## Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/YOUR_USERNAME/keras-mnist-comparison.git
cd keras-mnist-comparison
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebooks

```bash
jupyter notebook notebooks/
```

Run them in order: `01` → `02` → `03` → `04`

## Requirements

- Python 3.8+
- TensorFlow / Keras 2.x
- NumPy, Matplotlib, Pandas, Seaborn

## Project Structure

```
keras-mnist-comparison/
├── README.md
├── requirements.txt
└── notebooks/
    ├── 01_dense_model.ipynb
    ├── 02_conv2d_model.ipynb
    ├── 03_lstm_model.ipynb
    └── 04_comparison.ipynb
```

## Key Takeaways

- **Dense**: Simple and fast, surprisingly effective on flat image data
- **Conv2D**: Best accuracy — exploits spatial structure of images
- **LSTM**: Treats images as sequences of rows, competitive but slower

## License

MIT
