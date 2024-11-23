## A Generalized Semi-Supervised Learning Approach for 3D Medical Image Segmentation via Coarse Label Generation and Reconstruction

## Introduction
In semi-supervised medical image segmentation tasks, the annotation quality of complex 3D samples is often inconsistent, with variations arising from different annotators or physicians. These inconsistencies, along with the high cost of manual annotations, create challenges in fully capturing the 3D information from the samples. To address these issues, we propose the Coarse Label Generation and Reconstruction Network (CoGRNet), a novel method that integrates the concept of Dual-Plane Annotation (DPA) into the conventional Mean Teacher (MT) framework. Our approach involves manually annotating two orthogonal 2D slices and using spatial mapping to generate complete 3D coarse labels. This significantly reduces the burden of manual labeling. Additionally, by employing a Focus Area (FA) strategy to integrate labeled and unlabeled samples, our method promotes information exchange between the labeled and unlabeled datasets, improving the model's generalization ability. This approach ensures the preservation of fine details while achieving superior segmentation results.

## Requirements
This project is developed with the following versions:

- Python 3.9
- PyTorch 2.0.0+cu118

Other dependencies and their versions:
- tensorboardX 2.6.2.2
- tqdm 4.66.1
- scikit-image 0.22.0
- numpy 1.22.4
- pandas 2.1.4
- matplotlib 3.8.2
- opencv-python 4.9.0.80
- SimpleITK 2.3.1

## Usage
### Dataset Acquisition
- LA Dataset: [LA Dataset Link](https://github.com/yulequan/UA-MT/tree/master/data)
- kits19 Dataset: [kits19 Dataset Link](https://paperswithcode.com/dataset/kits19)
- Lits Dataset: [Lits Dataset Link](https://paperswithcode.com/dataset/lits17)
### Model Files
The model files can be downloaded from the following link:
- [Model Files](https://pan.baidu.com/s/19qFfX5eveS_yqRTK8s5Wuw?pwd=02ex)
  - Extraction Code: `02ex`

### Train
python ./code/utils/registration   #Label registration
python ./code/train.py  # Training on  dataset
### Test
python ./code/test.py  # Testing on  dataset

## Acknowledgements

We would like to express our gratitude to the Desco and Bidirectional Copy-Paste (BCP) teams for their inspiring work and valuable contributions. Their provided code and assistance have significantly influenced our project and helped shape its development. Thank you for your support and the foundational work that made this research possible.
Library Information
This project utilizes the following libraries:

tensorboardX: A library for TensorBoard support in PyTorch.
tqdm: A fast, extensible progress bar for Python.
scikit-image: A collection of algorithms for image processing.
numpy: A fundamental package for scientific computing in Python.
pandas: A data analysis and manipulation library.
matplotlib: A plotting library for creating static, animated, and interactive visualizations in Python.
opencv-python: A Python wrapper for the OpenCV library for computer vision tasks.
SimpleITK: A simplified layer built on top of the Insight Segmentation and Registration Toolkit (ITK).
