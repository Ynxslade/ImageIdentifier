# **SimCLR-Based Image Classifier**

This project utilizes **Self-Supervised Learning (SSL)** techniques to build an image classification model using TensorFlow and TensorFlow Hub. The TensorFlow Flowers dataset serves as a sample dataset for fine-tuning the pretrained SimCLR model for classification tasks.

## **Features**
- **Pretrained SimCLR Model**:
  - Integrated a SimCLR model from TensorFlow Hub for feature extraction.
  - Fine-tuned the model for the TensorFlow Flowers dataset.
- **Custom Preprocessing Pipeline**:
  - Applied advanced image augmentations such as color jitter, cropping, and random flipping.
- **Custom Training Loop**:
  - Built a custom training loop with a detailed logging callback for monitoring loss and accuracy.
- **Visualization**:
  - Visualized predictions with true labels using Matplotlib for interpretability.

## **Project Workflow**
1. **Dataset Loading**:
   - Leveraged TensorFlow Datasets (`tfds`) to load the `tf_flowers` dataset.
   - Preprocessed images by resizing and normalizing them for model input.

2. **Model Architecture**:
   - Used a pretrained SimCLR model as a feature extractor.
   - Added a fully connected layer for classifying images into five categories.

3. **Training**:
   - Fine-tuned the SimCLR model for 10 epochs using the Adam optimizer and categorical cross-entropy loss.

4. **Evaluation and Visualization**:
   - Evaluated predictions on a sample test batch.
   - Displayed predictions alongside true labels using Matplotlib.

## **Setup and Installation**

### **Requirements**
- Python 3.8+
- TensorFlow 2.x
- TensorFlow Hub
- TensorFlow Datasets
- Matplotlib
- NumPy

### **Install Dependencies**
1. Install the required libraries:
   ```bash
   pip install tensorflow tensorflow-hub tensorflow-datasets matplotlib numpy

## **Usage**

1. Run the training script:
   ```bash
   python train_image_classifier.py
2. View predictions:
The script outputs a visualization of predicted classes alongside true labels.
## **Dataset**

- **The TensorFlow Flowers Dataset includes five image categories**:
- Dandelion
- Daisy
- Tulips
- Sunflowers
- Roses
## **Visualizations**

- **Training Progress**:
- Monitors and logs training loss and accuracy per epoch.
Predictions:
Displays images with predicted and true labels.
## **References**

- TensorFlow Hub: SimCLR Model
- TensorFlow Datasets: Flowers Dataset
## **License**

-This project is licensed under the MIT License.
