# BanglaSummarization_colab

A Google Colab notebook that reproduces the Bengali/Bangla text summarization pipeline from the EACL 2021 paper by Nayeem et al. The notebook sets up both extractive and abstractive summarization models for the Bengali language using the `BengaliSummarization` codebase.

## Features

- Abstractive Bengali summarization using a pre-trained fastai-based sequence-to-sequence model (`export.pkl`)
- Extractive summarization using graph-based sentence ranking
- Uses `bnlm` (Bengali Language Model) for tokenization
- Colab-friendly setup: clones required repos and installs dependencies automatically

## Tech Stack

- Python 3
- PyTorch (`torch==1.2.0`)
- fastai
- `bnlm` (Bengali NLP library)
- `networkx==1.7`
- Google Colab

## Project Structure

| File | Description |
|---|---|
| `BengaliSummarization_EACL_2021.ipynb` | Main notebook: environment setup, model loading, summarization demo |

## Requirements

This notebook installs its own dependencies. Key packages:

```
torch==1.2.0
bnlm
networkx==1.7
fastai
```

## Usage

1. Open `BengaliSummarization_EACL_2021.ipynb` in Google Colab.
2. Mount Google Drive and place the pre-trained model at `/content/drive/MyDrive/Celloscope/BengaliSummarization/BenSumm/export.pkl`.
3. Run all cells in order.

## Reference

Nayeem et al., "EACL 2021 — Bengali Summarization"

## License

MIT
