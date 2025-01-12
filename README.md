## Trusted Mamba Contrastive Network for Multi-View Clustering
> **Authors:**
Jian Zhu, Xin Zou, Lei Liu*, Zhangmin Huang, Ying Zhang, Chang Tang, Li-Rong Dai. 

This repo contains the code and data of our ICASSP'2025 paper [Trusted Mamba Contrastive Network for Multi-View Clustering](https://arxiv.org/abs/2412.16487).

## 1. Abstract

Multi-view clustering can partition data samples into their categories by learning a consensus representation in an unsupervised way and has received more and more attention in recent years. However, there is an untrusted fusion problem. The reasons for this problem are as follows: 1) The current methods ignore the presence of noise or redundant information in the view; 2) The similarity of contrastive learning comes from the same sample rather than the same cluster in deep multi-view clustering. It causes multi-view fusion in the wrong direction. This paper proposes a novel multi-view clustering network to address this problem, termed as Trusted Mamba Contrastive Network (TMCN). Specifically, we present a new Trusted Mamba Fusion Network (TMFN), which achieves a trusted fusion of multi-view data through a selective mechanism. Moreover, we align the fused representation and the view-specific representation using the Average-similarity Contrastive Learning (AsCL) module. AsCL increases the similarity of view presentation from the same cluster, not merely from the same sample. Extensive experiments show that the proposed method achieves state-of-the-art results in deep multi-view clustering tasks.

## 2.Requirements

pytorch==1.12.1

numpy>=1.21.6

scikit-learn>=1.0.2

## 3.Datasets

The Synthetic3d, Prokaryotic, and MNIST-USPS datasets are placed in "data" folder. The others dataset could be downloaded from [cloud](https://pan.baidu.com/s/1XNWW8UqTcPMkw9NpiKqvOQ). key: data

## 4.Usage

- an example for train a new model：

```bash
python train.py
```
- an example  for test the trained model:
  
```bash
python test.py
```

- You can get the following output:

```bash
Epoch 290 Loss:430.929473
Epoch 291 Loss:422.919945
Epoch 292 Loss:423.580361
Epoch 293 Loss:429.665338
Epoch 294 Loss:417.705980
Epoch 295 Loss:425.192047
Epoch 296 Loss:428.146167
Epoch 297 Loss:419.057368
Epoch 298 Loss:423.789969
Epoch 299 Loss:416.932418
Epoch 300 Loss:418.947175
---------train over---------
Clustering results:
ACC = 0.9779 NMI = 0.9399 PUR=0.9779 ARI = 0.9516
Saving model...
```



## 5.Acknowledgments

Work&Code is inspired by [MFLVC](https://github.com/SubmissionsIn/MFLVC), [CONAN](https://github.com/Guanzhou-Ke/conan), [CoMVC](https://github.com/DanielTrosten/mvc) ... 

## 6.Citation

If you find our work useful in your research, please consider citing:

```latex
@article{zhu2024trusted,
  title={Trusted Mamba Contrastive Network for Multi-View Clustering},
  author={Zhu, Jian and Zou, Xin and Liu, Lei and Huang, Zhangmin and Zhang, Ying and Tang, Chang and Dai, Li-Rong},
  journal={arXiv preprint arXiv:2412.16487},
  year={2024}
}
```

If you have any problems, contact me via qijian.zhu@outlook.com.


