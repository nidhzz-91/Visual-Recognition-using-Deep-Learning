Overview
-This project implements a high-performance image classification pipeline using a customized ResNet-50 architecture. 
-The model integrates advanced training techniques such as data augmentation, mixed precision training, and cosine learning rate scheduling to achieve strong performance.

🧠 Key Features
✨ Custom ResNet-50 with improved pooling
✨ ConcatPool (Max + Avg pooling fusion)
✨ RandAugment for robust data augmentation
✨ Mixed Precision Training (AMP)
✨ Cosine Annealing Warm Restarts
✨ Label Smoothing for better generalization

Project Structure
├── data/
│   ├── train/
│   ├── val/
│   └── test/
├── results/
├── prediction.csv
├── prediction.zip
├── student_HW1.zip
├── friend_resnet50_best.pth
├── hw1.py
└── README.md


Clone Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name


Install Dependencies
pip install torch torchvision torchaudio

Dataset Setup
data/
Or extract using:
setup_data(tar_path, dest_path)

🏗️Model Architecture
Backbone: ResNet-50 (ImageNet pretrained)
Custom Layer:
ConcatPool2d (Adaptive Max + Avg Pooling)
Classifier:
Dropout (0.3)
Fully Connected Layer (100 classes)


