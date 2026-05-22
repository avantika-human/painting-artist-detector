# 🎨 Painting Artist Detector

A deep learning model that identifies the artist behind a painting. Upload any painting and the model predicts which of 10 iconic artists painted it — along with confidence scores.

## Demo
> Coming soon on Hugging Face Spaces 🤗

## Artists
The model can identify paintings by:
- Claude Monet
- Frida Kahlo
- Leonardo da Vinci
- Michelangelo
- Pablo Picasso
- Pierre-Auguste Renoir
- Rembrandt
- Salvador Dalí
- Sandro Botticelli
- Vincent van Gogh

## How It Works
- **Model**: ResNet18 pretrained on ImageNet, fine-tuned for artist classification
- **Dataset**: [Best Artworks of All Time](https://www.kaggle.com/datasets/ikarus777/best-artworks-of-all-time) — Kaggle
- **Training**: 49 paintings per artist, 20 epochs, Adam optimizer
- **UI**: Built with Gradio

## Limitations
- Small dataset (49 images per artist) limits generalization
- Artists with highly varied styles (e.g. Frida Kahlo) are harder to classify
- Can be improved with more data and a larger backbone (ResNet50)

## Tech Stack
- Python
- PyTorch & TorchVision
- Gradio
- Kaggle Datasets
