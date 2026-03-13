
# Dog Breed Recognition System

A deep learning–based dog breed recognition system that classifies images of dogs into their respective breeds using transfer learning with convolutional neural networks (CNNs).

This project evaluates and compares multiple pretrained CNN architectures to determine the most effective model for dog breed classification.

## Models Used

The following architectures were implemented and evaluated:

- ResNet50
- VGG16
- InceptionV3

These models leverage transfer learning from ImageNet to improve classification accuracy and training efficiency.

In this project, **InceptionV3 achieved the best performance (~82.8% accuracy)** on the Stanford Dogs dataset.

---

# Dataset

This project uses the **Stanford Dogs Dataset**, which contains images of **120 dog breeds**.

- Total Images: 20,580
- Total Classes: 120

Download the dataset:

http://vision.stanford.edu/aditya86/ImageNetDogs/images.tar

---

# Project Demo

https://youtu.be/Ic4UQqTkkCY

---

# Project Structure

Dog-Breed-Recognition/

- Test.py  
- Labels.py  

- ResNet50.py  
- VGG16.py  
- InceptionV3.py  

- ResNet50_Results.txt  
- VGG16_Results.txt  
- InceptionV3_Results.txt  

- Images/ (dataset folder)

### File Descriptions

| File | Description |
|-----|-------------|
| Group 27 (Null).pdf | Results and findings of the 3 models |
| ResNet50.py | Training script for the ResNet50 model |
| VGG16.py | Training script for the VGG16 model |
| InceptionV3.py | Training script for the InceptionV3 model |
| Labels.py | Contains dog breed labels |
| Test.py | Script used to test trained models |
| *_Results.txt | Evaluation results for each model |

---

# Installation

### 1. Clone the Repository

git clone https://github.com/Nann1207/Null.git  
cd Null

---

### 2. Download the Dataset

Download and extract the Stanford Dogs dataset:

http://vision.stanford.edu/aditya86/ImageNetDogs/images.tar

Place the extracted **Images** folder in the project directory.

Example structure:

project_folder/

-  Images/  
-  Test.py  
-  Labels.py  
-  ResNet50.py  
-  VGG16.py  
-  InceptionV3.py  

---

### 3. Install Dependencies

pip install tensorflow keras numpy matplotlib scikit-learn

---

# Running the Models

## Step 1 - Configure Dataset Path

Open:

ResNet50.py  
VGG16.py  
InceptionV3.py  

Update:

DATA_DIR = "C:\\Desktop\\Folder\\Images"

---

## Step 2 - Train the Models

python ResNet50.py

or

python VGG16.py

or

python InceptionV3.py

---

## Step 3 - Configure Test Script

Open **Test.py** and update:

MODEL_PATH  
LABELS_PATH

Example:

MODEL_PATH = "C:\\Desktop\\Folder\\InceptionV3model.keras"  
LABELS_PATH = "C:\\Desktop\\Folder\\Labels.py"

---

## Step 4 - Run Test Script

python Test.py

---

# Results

Model results are provided in:

ResNet50_Results.txt  
VGG16_Results.txt  
InceptionV3_Results.txt  

Example metrics (InceptionV3):

| Metric | Score |
|------|------|
| Accuracy | 0.8283 |
| Precision | 0.8332 |
| Recall | 0.8283 |
| F1 Score | 0.8273 |

---

# Methodology

Key techniques used:

- Transfer learning with pretrained CNN architectures
- Data augmentation for improved generalization
- Fine-tuning model layers
- Evaluation using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - Confusion matrix

---

# Limitations

- Similar-looking breeds may be misclassified
- Image quality and backgrounds can affect predictions
- Dataset imbalance across breeds
- Performance may vary on real-world images

Future improvements may include:

- Larger datasets
- Additional CNN architectures
- Improved preprocessing
- More training compute

---

# Authors

Group 27 (Null)

- Vania Graciella Kwee
- Niruba Annriea Kichor Sagayaradje  
- Joshe D/O Chantiramugan 
- Wong Poh Yee  
- Teng Wei Chee  
- Keeve Wong Ye Kai  

---

# 📚 References

Stanford Dogs Dataset  
http://vision.stanford.edu/aditya86/ImageNetDogs/



# NOTE: The output files are provided as .txt files.

