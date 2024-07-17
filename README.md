# drowsy-driver-detection
## description
The following is an academic project made for the CSE4006 Deep Learning class, that compares the efficacy of two CNN image processing deep learning models.

1 in 25 adult drivers reported falling asleep while driving in the past 30 days in a CDC survey. Drowsy driving is dangerous and contributed to 91,000 crashes in 2017, resulting in 50,000 injuries and nearly 800 deaths.

Detecting driver drowsiness is crucial for preventing such accidents and saving lives. The goal is to implement a deep learning model that uses computer vision to analyze facial expressions and identify signs of drowsiness (closed eyes, yawning) versus alertness (open eyes, no yawn).

I designed models using the LeNet and VGG19 architectures and evaluated their accuracy and effectiveness in detecting driver drowsiness.
## Table of Contents
- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Models](#models)
- [Results](#results)
## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/vyomaa/drowsy-driver-detection.git
    ```
2. Navigate to the project directory:
    ```sh
    cd drowsy-driver-detection
    ```
3. Upload your kaggle.json file into the project directory (That you can get from your Kaggle account settings)
   
## Usage

1. Open the Jupyter notebook
2. Run the cells in the notebook to see the analysis and results.

## Dataset

The dataset used is [Drowsiness_dataset](https://www.kaggle.com/datasets/dheerajperumandla/drowsiness-dataset). This dataset contains images of the driver in states of drowsiness and non-drowsiness

1. Closed (726 images)
2. Open (726 images)
3. no_yawn (725 images)
4. yawm (723 images)

## Models

The following models were used in this project:
- **LeNet Model**: Developed by Yann LeCun, it is one of the first convolutional neural networks (CNNs) and was designed for handwritten digit recognition. The architecture of LeNet consists of two sets of convolutional and average pooling layers, followed by a fully connected layer and an output layer with softmax activation.

  ![image](https://github.com/user-attachments/assets/1dcf0b19-5475-4a94-9fe9-45599bbab975)

- **VGG19**: It is a deep convolutional neural network model developed by the Visual Geometry Group (VGG) at the University of Oxford. It's architecture consists of 16 convolutional layers with small receptive fields (3x3 filters) and 3 fully connected layers. The network also includes max-pooling layers after every few convolutional layers.

  ![image](https://github.com/user-attachments/assets/9b8bfe4d-c48c-4633-8458-67981df08a4f)

## Results

1. LeNet

<p align="center">
  <img src="https://github.com/user-attachments/assets/0cbf4e7d-0c17-48fd-bdf7-9caa0c38a7fc" alt="lenet_accuracy" width="45%" style="display: inline-block; margin-right: 10px;">
  <img src="https://github.com/user-attachments/assets/05a3d9a3-b18c-409e-acd3-4ecc91429724" alt="lenet_loss" width="45%" style="display: inline-block;">
</p>

2. VGGNet-19

<p align="center">
  <img src="https://github.com/user-attachments/assets/f468cf3a-b225-41fd-ad4d-61adb0611e4f" alt="vgg19_accuracy" width="45%" style="display: inline-block; margin-right: 10px;">
  <img src="https://github.com/user-attachments/assets/929979f6-6b35-4f17-9a46-0d4b755f91b5" alt="vgg19_loss" width="45%" style="display: inline-block;">
</p>


### Accuracy Comparison of Drowsiness Detection Methods

Authors  | Method | Results
-------------------|------------------|---------------
[1] GWAK ET AL.      | ENSEMBLE MACHINE LEARNING     | 65.2 %
[2] JABBAR ET AL.      | CNN     | 83.33 %
[3] MEHTA ET AL. | EYE ASPECT RATIO AND EYE CLOSURE RATIO | 84 %
[4] KEPESIOVA ET AL. | CONV GRNN, CNN | 84.41 %
[5] DUA ET AL. | ALEXNET, VGG-FACENET, FLOWIMAGENET, RESNET | 85 %
[6] AYTEKIN ET AL. | TRANSFER LEARNING VGG16 | 91 %
METHOD1 | LeNet | 94.46 %
METHOD2 | VGGNet-19 | 99.31% %

References
[1] J. Gwak, A. Hirao, and M. Shino, “An investigation of early detection of driver drowsiness using ensemble machine learning based on hybrid sensing”,  Appl. Sci.,  vol.  10, no. 8,  Apr.  2020, Art no. 2890. https://doi.org/10.3390/app10082890

[2] R. Jabbar, M. Shinoy, M. Kharbeche, K. Al-Khalifa, M. Krichen, and K. Barkaoui, “Driver drowsiness detection model using convolutional neural networks techniques for android application”, in Proceedings of the 2020 IEEE  International  Conference  on  Informatics,  IoT,  and  Enabling Technologies, Doha, Qatar, May 2020, pp. 2–5. https://doi.org/10.1109/ICIoT48696.2020.9089484  

[3] S. Mehta, S. Dadhich, S. Gumber,  and A. J. Bhatt, “Real-time driver drowsiness detection system using eye aspect ratio and eye closure ratio”, in Proceedings of international conference on sustainable computing in science,  technology  and  management  (SUSCOM), Jaipur,  India,  Feb. 2019. https://doi.org/10.2139/ssrn.3356401

[4] Z. Kepesiova, J. Ciganek,  and S. Kozak, “Driver drowsiness detection using convolutional neural networks”, in 2020 Cybernetics & Informatics (K&I),  Velke Karlovice, Czech Republic,  Mar. 2020, pp. 1–6. https://doi.org/10.1109/KI48306.2020.9039851

[5] M. Dua, R. Singla, S. Raj,  and A. Jangra, “Deep CNN models-based ensemble approach to driver drowsiness detection”, Neural Computing and Applications, vol. 33, no. 8, pp. 3155–3168, Jul. 2021.  https://doi.org/10.1007/s00521-020-05209-7

[6] Alper Aytekin, Vasfiye Mençik, "Detection of Driver Dynamics with VGG16 Model", in Applied Computer Systems 27(1):83-88, June 2022. http://dx.doi.org/10.2478/acss-2022-0009

Image Credit: Google
