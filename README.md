# Complex Embeddings with GloVe for Text Classification

## Overview

This project demonstrates the use of complex embeddings for text classification using TensorFlow and Keras. The complex embedding layer integrates amplitude and phase components to represent word embeddings in a novel way. These embeddings are treated as elements of a Hilbert space, allowing us to leverage the mathematical properties of Hilbert spaces for improved text classification. Pre-trained GloVe embeddings are used to initialize the complex embeddings.

## Features

- **Custom Complex Embedding Layer:** A Keras custom layer that utilizes both amplitude and phase components for word embeddings, with embeddings represented in a Hilbert space.
- **GloVe Embeddings:** Pre-trained GloVe embeddings are used to initialize the complex embeddings.
- **Hilbert Space Integration:** Embeddings are treated as elements of a Hilbert space, incorporating mathematical properties to enhance performance.
- **IMDB Dataset:** A popular dataset for sentiment analysis, used here for text classification.
- **Model Architecture:** A model that includes complex embeddings, global average pooling, dropout, and a dense output layer.

## Prerequisites

- Python 3.x
- TensorFlow 2.x
- NumPy
- Requests
- Gensim

You can install the required packages using `pip`:

```bash
pip install tensorflow numpy requests gensim
```
## Project Structure
```
.
├── README.md
├── glove/                  # Directory for storing GloVe embeddings
├── main.py                 # Main script for downloading data, training, and evaluation
└── requirements.txt        # Required Python packages

```


## Hilbert Space and Complex Embeddings
In this project, the complex embeddings are modeled as elements of a Hilbert space. A Hilbert space is a complete inner product space, which allows for the rigorous mathematical treatment of complex vectors. The use of Hilbert space concepts enables the incorporation of both amplitude and phase information into the embeddings, potentially leading to improved performance in text classification tasks.

### Usage
- Download and Prepare GloVe Embeddings:
    The script will automatically download and extract the GloVe embeddings if they are not already present.

- Load the IMDB Dataset:
    The script loads and preprocesses the IMDB dataset, including tokenization and padding.

- Define and Train the Model:
    The model is built using a custom complex embedding layer, compiled, and trained on the IMDB dataset.

- Process and Analyze Test Sentences:
    Example sentences can be processed and analyzed using the trained model.



## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements:
- GloVe: [Global Vectors for Word Representation](https://nlp.stanford.edu/projects/glove/)
- IMDB Dataset: [IMDB Reviews](https://www.imdb.com/interfaces/)
- Hilbert Space Theory: [Introduction to Hilbert Spaces](https://en.wikipedia.org/wiki/Hilbert_space)
