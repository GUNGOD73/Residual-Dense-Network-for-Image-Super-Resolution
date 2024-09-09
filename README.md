# Residual Dense Network for Image Super Resolution
This repository contains the implementation of a Residual Dense Network (RDN) for various image restoration tasks, such as image super-resolution, image denoising, image deblurring, and compression artifact reduction. The RDN model utilizes Residual Dense Blocks (RDBs) to extract and exploit hierarchical features and employs local and global feature fusion techniques for effective learning.

## Introduction
Image restoration (IR) aims to recover high-quality images from low-quality or degraded measurements. IR plays a crucial role in several computer vision applications. Despite the advancements in deep learning, existing methods often fail to fully utilize hierarchical features from low-quality images, leading to suboptimal results.

This project introduces a novel Residual Dense Network (RDN), which:

- Fully exploits hierarchical features from all convolutional layers.
- Uses Residual Dense Blocks (RDBs) to capture local features.
- Applies local and global feature fusion for adaptive learning.
- Demonstrates superior performance in image super-resolution, denoising, deblurring, and artifact reduction tasks.

## Features
- Residual Dense Network (RDN) architecture for superior image restoration.
- Residual Dense Blocks (RDBs) to extract and utilize hierarchical features.
- Local and Global Feature Fusion to learn more effective representations.
- Applicable to multiple image restoration tasks:
    - Super-resolution
    - Denoising
    - Deblurring
    - Compression artifact reduction
- Outperforms state-of-the-art methods on both benchmark and real-world datasets.


## Architecture
The RDN architecture is built with the following key components:

- Residual Dense Block (RDB): Captures local features with residual learning, allowing hierarchical feature extraction 
  across all convolutional layers.
- Contiguous Memory Mechanism: Direct connections between preceding and current RDBs.
- Local Feature Fusion (LFF): Fuses features within each RDB.
- Global Feature Fusion (GFF): Combines features from all RDBs adaptively to learn better global features.


## Datasets

The RDN model was trained and tested on the following datasets:

- DIV2K: High-quality images for super-resolution tasks.
- Set5/Set14: Common benchmark datasets for image super-resolution.
- BSD500: Dataset for denoising tasks.
