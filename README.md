# Neural Cryptography

A neural network-based cryptographic system where Alice and Bob learn to communicate securely while Eve tries to intercept their messages.

## Overview

Three neural networks engage in adversarial training:
- **Alice**: Encrypts messages
- **Bob**: Decrypts Alice's messages  
- **Eve**: Attempts to break the encryption

## Setup

```bash
git clone https://github.com/your-username/neural-cryptography.git
cd neural-cryptography
pip install -r requirements.txt
```

## Usage

Train the system:
```bash
python scripts/train_neural_crypto.py
```

Run interactive demo:
```bash
jupyter notebook notebooks/neural_cryptography_demo.ipynb
```

## Project Structure

```
neural-cryptography/
├── data/        # Input messages and datasets
├── models/      # Neural network architectures
├── notebooks/   # Experiments and demos
├── scripts/     # Training and evaluation scripts
├── requirements.txt
└── README.md
```

## Requirements

- Python 3.8+
- TensorFlow 2.0+
- NumPy
- Matplotlib

## License

MIT License
