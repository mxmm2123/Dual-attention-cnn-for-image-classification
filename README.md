# Dual Attention for Image Classification

### Introduction
This project combine Spatial attention from the [BAM model](https://arxiv.org/pdf/1807.06514.pdf) with Frequency Channel Attention from [FcaNet network](https://arxiv.org/abs/2012.11879) to improve CNN model for medical image classification.

Use Spatial attention in BAM:

![][1]

  [1]: ./images/BAM.png

Frequency Channel Attention:

![][2]

  [2]: ./images/fcanet.png

### Denpendency
* python3.10
* tensorflow2.15
* The code is work on Ubuntu 20.04.6 LTS

### Recommended

* Ubuntu 20.04 with tensorflow GPU edition
* Kaggle or Colab free version.
* I implement code on [Colab Notebook](https://colab.research.google.com/drive/1qRF33PsNyHIJiU7PeKFPQx0U1dJc7ch8?usp=sharing).

### Getting Started

```bash
git https://github.com/mxmm2123/Dual-attention-cnn-for-image-classification.git
```
#### Dataset

* [ISIC 2018 task 3](https://challenge.isic-archive.com/data/#2018) - Skin lesion diagnosis dataset. There are 10,015 images in this dataset with seven different categories.

* [KvasirPogorelov dataset](https://dl.acm.org/do/10.1145/3193289/full/) - Dataset includes 4000 endoscopic gastrointestinal diseases and comprises eight classes, each containing 500 images.

You can use my [proccessed data](https://drive.google.com/drive/folders/1-KCyJa5gLoVEm61aud7xOcyXaaix_vlt?usp=drive_link). Your dataset structure should like:

```bash
./data
├── train
│   ├── class 1
│   │   ├── image 1
│   │   ├── image 2
│   │   └── ...
│   ├── class 2
│   └── ...
└── test
    ├── class 1
    │   ├── image 1
    │   ├── image 2
    │   └── ...
    ├── class 2
    └── ...
```

