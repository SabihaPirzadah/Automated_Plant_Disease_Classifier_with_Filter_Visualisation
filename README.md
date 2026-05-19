# Plant Disease Classification using Deep Learning

## Project Overview
This project focuses on detecting and classifying plant diseases using deep learning techniques. The system takes an input image of a plant leaf and predicts the plant type, disease name, and confidence score.

The main objective is to assist farmers and researchers by providing an automated disease detection system.

---

## Features
- Image-based plant disease classification
- Supports 38 different plant disease classes
- Uses Deep Learning (CNN & Transfer Learning)
- Real-time image prediction in Google Colab
- Displays confidence score with prediction
- Image visualization using OpenCV filters

---

## Models Used

### CNN from Scratch
- Custom 3-layer Convolutional Neural Network
- Accuracy: 82.84%

### MobileNetV2 (Frozen)
- Pretrained on ImageNet
- Only classification head trained
- Accuracy: 88.28%

### MobileNetV2 (Fine-Tuned)
- Last 30 layers unfrozen
- Best performing model
- Accuracy: 92.06%

---

## Technologies Used
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Dataset
- Plant disease dataset (38 classes)
- Includes healthy and diseased leaf images
- Data augmentation applied

---

## Installation

Install required libraries using pip:

```bash
pip install tensorflow opencv-python numpy pandas matplotlib seaborn scikit-learn kaggle
```

---

## How to Run the Project

1. Open Google Colab
2. Upload the `.ipynb` file
3. Mount Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
```

4. Add Kaggle API credentials
5. Run all cells step by step:
   - Data loading
   - Preprocessing
   - Model training
   - Evaluation
   - Prediction

---

## Image Prediction

Steps:
- Upload leaf image
- Image is resized to 128x128
- Model predicts:
  - Plant Name
  - Disease Name
  - Confidence Score

---

## Results

| Model                     | Accuracy |
|--------------------------|----------|
| CNN from Scratch         | 82.84%   |
| MobileNetV2 Frozen       | 88.28%   |
| MobileNetV2 Fine-Tuned   | 92.06%   |

Best Model: MobileNetV2 Fine-Tuned

---

## Challenges
- Tomato diseases are visually similar
- Requires GPU for training
- Limited training epochs

---

## Limitations
- Not optimized for mobile devices
- Dataset is augmented (not fully real-world)
- Lower resolution images (128x128)

---

## Future Improvements
- Use higher resolution images (224x224)
- Train for more epochs
- Try advanced models (EfficientNet, ResNet)
- Collect real-world dataset

---

## Conclusion
The project shows that transfer learning significantly improves plant disease classification accuracy. The fine-tuned MobileNetV2 model achieved the best performance.

---

## Contributors
- Sabiha Pirzadah  
- Hafsa Naz  
- Kainat Moin  
- Saira Jabeen  

---

## License
This project is for academic purposes.
