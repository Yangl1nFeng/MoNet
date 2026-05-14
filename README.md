# MoNet 🧙‍♀️
Multimodal Nested Learning for Decoupled and Coordinated Optimization (ICML 2026 Spotlight Paper Pytorch Code)

![intro](./imgs/main.png)

## TL;DR
This paper proposes an Information-Balanced Multimodal Learning (IBML) framework, which explains multimodal optimization imbalance as uneven preservation of complementary information and addresses it through nested BIO optimization and TCM task-complexity modulation, enabling balanced multimodal fusion and superior performance across diverse tasks.

## Todo List
✅ Dataset
Coming in 1-2 weeks...
🈚️ Method Code
🈚️ Checkpoints

## 📕 Data
Following [TPAMI 2026: IBML](https://github.com/QinYang79/IBML).
### Audio-Vision Recognition
- CREMAD and AVE:

See data_process.zip

Read or run `bash run.sh`

- avsbench and VGGSound50

See [here](https://modelscope.cn/datasets/yangsss/IBML_data).

```
IBML_data
│
├── avsbench
│     └── avsbench.tar.gz
│
└── VGGSound50
      ├── Image-01-FPS.tar.gz
      ├── audios.tar.gz
      ├── train.txt
      └── test.txt
```

### Image-Text Classification
- food101 and MVSA

See data_process.zip

Read or run `bash run.sh`

### 2D-3D Classification
- 3D MNIST

We have provided the preprocessed data for you on [Dropbox](https://www.dropbox.com/scl/fo/zqgf44jsdqflge81nk1ml/ABSD8fj9F0_anJWmk_M2Mio?rlkey=zqohocqvfj9ho2oqvclvkq9kk&e=1&dl=0). Please place it under `data\3D_MNIST`.

If you use raw data [Kaggle-3D MNIST](https://www.kaggle.com/datasets/daavoo/3d-mnist), suitable data augmentation can bring the performance of the method to a higher level.

- ModelNet 40  

We have also provided the preprocessed 3D data for you on [Dropbox](https://www.dropbox.com/scl/fo/2oyahbyp4scnkvb5k96sk/h?rlkey=ujg89pc3sturtbtyozhipgiew&e=1&dl=0). Please place it under `data\ModelNet40`. In addition, the 180-view 2D images are large. Please refer to this link (https://github.com/LongLong-Jing/Cross-Modal-Center-Loss/issues/2) to download them, and then place them under `data\ModelNet40`.

All data processing procedures refer to:  
https://github.com/penghu-cs/RONO  
and  
https://github.com/LongLong-Jing/Cross-Modal-Center-Loss  

If you encounter any issues, please consult the guidance or issues sections of these projects.

## 📦 Requirements

- python>=3.8
- torch
- torchvision
- numpy
- torchtext
- tensorboard
- tqdm

## 🔨 Training and Testing 
After placing the data in the `./data` directory, you can begin training and testing. Specifically, the paper has the following three tasks:
### Audio-Vision Recognition
Modify the appropriate configuration, then run:

### Image-Text Classification
Modify the appropriate configuration, then run:

### 2D-3D Classification
Modify the appropriate configuration, then run:

## Reference 🤗
If this paper is helpful for your research, please cite:
```bibtex
coming soon...
```
