# Physics-informed DeepCT: Sinogram Wavelet Decomposition Meets Masked Diffusion (SWARM)
[![arXiv](https://img.shields.io/badge/arXiv-2501.09935-b31b1b.svg)](https://arxiv.org/abs/2501.09935)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
This repository contains the official implementation of the paper **"Physics-informed DeepCT: Sinogram Wavelet Decomposition Meets Masked Diffusion"**.
> [cite_start]**Note:** The source code is available at [https://github.com/yqx7150/SWARM](https://github.com/yqx7150/SWARM)[cite: 2325].

## Abstract
Abstract— Diffusion models have demonstrated strong potential in sparse-view computed tomography (SVCT) reconstruction. However, their generalization ability is often constrained when trained on limited sample spaces, leading to performance degradation when encountering unseen data. This typically leads to image blurring, loss of structural details, and cross-region inconsistencies. To address these challenges, we propose a Sinogram-based Wavelet random decomposition And Random mask diffusion Model (SWARM) for SVCT reconstruction. Specifically, introducing a random mask strategy in the sinogram effectively expands the limited training sample space. This enables the model to learn a broader range of data distributions, enhancing its understanding and generalization of data uncertainty. In addition, we designed a wavelet-based random training mechanism for sinogram high-frequency components, enabling the model to capture structural details in different frequency bands and enhancing the richness and structural consistency of the representations. Two stage iterative reconstruction method is adopted to ensure the global consistency of the reconstructed image while refining the details. Compared with other state-of-the-art reconstruction methods, SWARM can increase the PSNR by 3.59 dB on average, the SSIM by 0.69%, and reduce the MSE by 55.40%. These experimental results indicate that SWARM has great potential in the field of sparse-view CT image reconstruction.

Index Terms— Sparse-view CT, random mask, sinogram wavelet decomposition, diffusion model.

## Methond Overview
<p align="center">
  <img src="assets/performance_comparison.png" alt="Different training strategies and influence of sinogram in deeplearning." width="800">
  <br>
  <em>Figure 1: Different training strategies and influence of sinogram in deep learning. (a) Distribution of training data in a closed data space; (b) The distribution of the data obtained through the mask extension method in the extended data space; (c) The generation process of the random mask and how it is embedded in the data..</em>
</p>







## Citation
```bibtex
If you find this work useful, please cite our paper:
@article{zhou2025swarm,
  title={Physics-informed DeepCT: Sinogram Wavelet Decomposition Meets Masked Diffusion},
  author={Zhou, Zekun and Liu, Tan and Yu, Bing and Gong, Yanru and Tao, Xi and Shi, Liu and Liu, Qiegen},
  journal={arXiv preprint arXiv:2501.09935},
  year={2025}
}
