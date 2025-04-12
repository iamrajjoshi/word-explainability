# word-explainability

"Representing visual classification as a linear combination of words" - Implementation for skin cancer classification using HAM10000 dataset

## Overview

This repository implements the approach described in the paper "Representing visual classification as a linear combination of words" (Agarwal, Semenov, & Lotter, 2023). The method uses a vision-language model (CLIP) to identify language-based descriptors for visual classification tasks, providing intuitive explainability.
The implementation focuses on skin cancer classification using the HAM10000 dataset, demonstrating how complex visual classification tasks can be represented through human-understandable language.

## Features

- Utilizes the CLIP model to extract visual features from dermatoscopic images
- Trains a linear classifier on top of CLIP embeddings for melanoma detection
- Represents the classifier as a linear combination of descriptive words
- Identifies prototypical examples for each descriptive word
- Includes simulation of the reader study described in the paper
- Supports both the original word set from the paper and an extended domain-specific word set

## Requirements

```bash
torch
clip
numpy
pandas
scipy
tqdm
scikit-learn
matplotlib
seaborn
pillow
```

## Usage

The main implementation is provided as a Jupyter/Google Colab notebook that can be run directly with the HAM10000 dataset.

## Data

This implementation uses the HAM10000 dataset, a collection of 10,015 dermatoscopic images of pigmented skin lesions across seven disease categories. For this implementation, we focus on the binary classification task of distinguishing melanoma (malignant) from nevi (benign).

## Citation

If you use this implementation, please cite the original paper:

```bibtex
@misc{agarwal2023representingvisualclassificationlinear,
      title={Representing visual classification as a linear combination of words}, 
      author={Shobhit Agarwal and Yevgeniy R. Semenov and William Lotter},
      year={2023},
      eprint={2311.10933},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2311.10933}, 
}
```

## Acknowledgments

The authors of the original paper
The HAM10000 dataset creators and contributors
The CLIP model developers at OpenAI
