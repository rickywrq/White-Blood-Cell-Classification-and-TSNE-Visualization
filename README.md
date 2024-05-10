# White-Blood-Cell-Classification-and-TSNE-Visualization
## Overview
### Example of cells
![Alt text](assets/cells.png?raw=true "Title")
### T-SNE visualization
![Alt text](assets/tsne.png?raw=true "Title")

## Download the dataset
https://universe.roboflow.com/liu-6c2az/blood-cells-uf28o/health

## Unzip the dataset zip
```unzip blood\ cells.v1i.coco.zip -d dataset_original```

## Preprocess the dataset
run the jupyter notebook: `pre_process_dataset.ipynb`

## Train the Model
`transfer_learning_tutorial.ipynb`
* Code adapted from: https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html

ckpt: A pre-trained ckpt can be found [here](https://github.com/rickywrq/White-Blood-Cell-Classification-and-TSNE-Visualization/releases/download/ckpt/model_wbc_resnet50_v2.pth). Please download and put it in `ckpt/`.

## Visualization
`wbc_resnet_tsne.ipynb`
* Code adapted from: https://learnopencv.com/t-sne-for-feature-visualization/