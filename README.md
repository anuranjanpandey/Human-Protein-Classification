# Human-Protein-Classification

This is my submission of Kaggle competition [Zero to GANs - Human Protein Classification](https://www.kaggle.com/c/jovian-pytorch-z2g/overview).

## Description

<img src="https://user-images.githubusercontent.com/53137708/119226625-b9304880-bb27-11eb-8944-dbf40d35da48.png" width="350" height="350"/>  <img src="https://user-images.githubusercontent.com/53137708/119226629-bb92a280-bb27-11eb-9502-3e284f9bd7ce.png" width="350" height="350"/>  

In this competition, I have developed a model capable of classifying mixed patterns of proteins in microscope images. Images visualizing proteins in cells are commonly used for biomedical research, and these cells could hold the key for the next breakthrough in medicine. However, thanks to advances in high-throughput microscopy, these images are generated at a far greater pace than what can be manually evaluated. Therefore, the need is greater than ever for automating biomedical image analysis to accelerate the understanding of human cells and disease.

This is a multilabel image classification problem, where each image can belong to several classes. The class labels are as follows:

0. 'Mitochondria',
1. 'Nuclear bodies',
2. 'Nucleoli',
3. 'Golgi apparatus',
4. 'Nucleoplasm',
5. 'Nucleoli fibrillar center',
6. 'Cytosol',
7. 'Plasma membrane',
8. 'Centrosome',
9. 'Nuclear speckles'

## Dataset

Dataset contains 512x512 resolution images of 3 channels (RGB). Images are in PNG format. Train set contains - 19236 images Test set contains - 8243 images.

## Prediction

We are predicting protein organelle localization labels for each sample. There are in total 10 different labels present in the dataset. The dataset is acquired in a highly standardized way using one imaging modality (confocal microscopy). However, the dataset comprises 10 different cell types of highly different morphology, which affect the protein patterns of the different organelles. Each image can have 1 or more labels associated to them.
