# 🧠 Makemore

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg) 
![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![Status](https://img.shields.io/badge/status-Active-success.svg)

---

## 📋 Table of Contents
- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Models Supported](#-models-supported)
- [Sample Outputs](#-sample-outputs)
- [Configuration](#-configuration)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 Overview

**Makemore** is an autoregressive **character-level language model** that generates new data based on a given dataset.

It takes a simple text file (one sample per line) and learns patterns to generate **new realistic outputs**.

> 💡 Example: Train on baby names → Generate new unique names that *sound real but don’t exist.*

---

## ✨ Features

✅ **Multiple Model Architectures**
- Bigram
- MLP
- RNN / LSTM / GRU
- Transformer (default)

✅ **Text Generation**
- Character-level generation
- Autoregressive modeling
- Dataset-driven output

✅ **Lightweight & Hackable**
- Single-file implementation
- Minimal dependencies (PyTorch only)
- Easy to modify and experiment

✅ **Educational Focus**
- Understand deep learning fundamentals
- Learn sequence modeling from scratch
- Explore GPT-like architectures in simple form

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| **Language** | Python |
| **Framework** | PyTorch |
| **Model Types** | Bigram, MLP, RNN, LSTM, GRU, Transformer |
| **Training** | CPU / GPU supported |

---

## ⚙️ Installation

### Prerequisites
- Python 3.8+
- pip

### Step-by-Step Setup

1. **Clone the Repository**
```bash
git clone https://github.com/Birabhadra/Makemore.git
cd makemore
```

2.Install Dependencies
```bash
pip install torch
```
🚀 Usage
📂 Prepare Dataset

Create a .txt file where each line is a training example:
```
emma
olivia
ava
isabella
sophia
charlotte
```
## 🏋️ Train the Model
```
python makemore.py -i names.txt -o names
```
Saves logs, checkpoints, and outputs in the names/ directory

Default model: Tiny Transformer (~200K parameters)

## 🎲 Generate Samples
```
python makemore.py -i names.txt -o names --sample-only
```
Loads the best trained model

Generates outputs on demand

## 🧠 Models Supported

| Model       | Description                                      |
|------------|--------------------------------------------------|
| Bigram     | Predicts next character using frequency counts   |
| MLP        | Feedforward neural network                       |
| CNN        | WaveNet-style architecture *(in progress)*       |
| RNN        | Recurrent neural network                         |
| LSTM       | Long Short-Term Memory                           |
| GRU        | Gated Recurrent Unit                             |
| Transformer| Attention-based model *(default)*                |

## 🧪 Sample Outputs
Generated from a names dataset:
```
dontell
khylum
camatena
aeriline
najlah
sherrith
ryel
irmi
taislee
mortaz
akarli
maxfelynn
biolett
zendy
laisa
halliliana
```
✨ These outputs are unique, realistic, and dataset-inspired


## 🧩 Use Cases

- 👶 Baby name generation
- 🏢 Startup/company name ideas
- 🎮 Game character naming
- 📚 Synthetic text generation
- 🧪 NLP experimentation


## 🤝 Contributing
Contributions are welcome!

Steps:
```bash
git checkout -b feature/your-feature
git commit -m "feat: add your feature"
git push origin feature/your-feature
```
Then open a Pull Request 🚀
