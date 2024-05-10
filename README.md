# White Blood Cell Classification and t-SNE Visualization

## Project Overview
This project focuses on classifying white blood cells (WBCs) using deep learning and visualizing their features using t-SNE (t-distributed Stochastic Neighbor Embedding). The white blood cells analyzed include:

- **BA (Basophils):** White blood cells involved in immune responses, particularly allergic reactions and parasitic infections.
- **EO (Eosinophils):** Combat parasitic infections and contribute to allergic reactions.
- **LY (Lymphocytes):** Provide immune defense. Different types include B cells, T cells, and NK (natural killer) cells.
- **PLATELET (Thrombocytes):** Vital for blood clotting and wound healing.
- **SNE (Segmented Neutrophils):** The most abundant mature neutrophils that ingest bacteria and fungi.

### Sample Cell Images
![Sample Cells](assets/cells.png?raw=true "Example of Different White Blood Cells")

### t-SNE Visualization
![t-SNE Visualization](assets/tsne.png?raw=true "t-SNE Feature Visualization")

## Getting Started
Follow these steps to set up and execute the project:

### 1. Download the Dataset
You can access the blood cell dataset [here](https://universe.roboflow.com/liu-6c2az/blood-cells-uf28o/health).

### 2. Unzip the Dataset
Extract the contents of the downloaded `.zip` file to a designated folder.
```bash
unzip blood\ cells.v1i.coco.zip -d dataset_original
```

### 3. Preprocess the Dataset
Run the `pre_process_dataset.ipynb` Jupyter notebook to preprocess the data before training.

### 4. Train the Model
Use the `transfer_learning_tutorial.ipynb` notebook to train the classification model. This notebook is adapted from the [PyTorch transfer learning tutorial](https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html).

A pre-trained model checkpoint is available [here](https://github.com/rickywrq/White-Blood-Cell-Classification-and-TSNE-Visualization/releases/download/ckpt/model_wbc_resnet50_v2.pth). Download it and place it in the `ckpt/` directory.

### 5. Visualization
Use the `wbc_resnet_tsne.ipynb` notebook to visualize the extracted features using t-SNE. The code is adapted from the [tutorial](https://learnopencv.com/t-sne-for-feature-visualization/).