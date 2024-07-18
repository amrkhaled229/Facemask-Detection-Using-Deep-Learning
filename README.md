# Facemask Detection Using Deep Learning

This project implements and compares six different Convolutional Neural Network (CNN) models for facemask detection using the "Face Mask Dataset" from Kaggle. The models include VGG16, VGG19, a custom CNN, ConvNeXtTiny, ResNet101, and ResNet152. Among these, VGG19 showed the best performance.

## Project Overview

The COVID-19 pandemic has highlighted the importance of wearing facemasks to prevent virus transmission. Automatic facemask detection systems can aid in enforcing mask-wearing regulations in public spaces. This project presents a comprehensive comparative analysis of six CNN models for facemask detection, aiming to identify the most effective model based on performance metrics such as accuracy, precision, recall, and F1 score.

## Models Implemented
- *VGG16*
- *VGG19*
- *Custom CNN*
- *ConvNeXtTiny*
- *ResNet101*
- *ResNet152*

## Dataset

The dataset used is the "Face Mask Dataset" by Omkar Gurav on Kaggle. It contains images categorized into 'with mask' and 'without mask'.

## Preprocessing

- Images resized to 128x128 pixels.
- Data augmentation techniques applied: rotation, width shift, height shift, shear, zoom, and horizontal flip.

## Training

- Models trained using TensorFlow and Keras.
- Adam optimizer with a learning rate of 0.001.
- Binary cross-entropy loss function.
- Early stopping and callbacks to prevent overfitting.
- Maximum of 50 epochs with early stopping typically around 10-20 epochs.

## Results

The VGG19 model achieved the best performance with:
- *Accuracy*: 95.75%
- *Precision*: 98.19%
- *Recall*: 93.34%
- *F1 Score*: 95.70%

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/facemask-detection.git](https://github.com/Mounir62/Facemask_Detection_Model.git
Change into the project directory:
bash
Copy code
cd facemask-detection
Install the required packages:
bash
Copy code
pip install -r requirements.txt
Usage
Download and unzip the dataset from Kaggle:

bash
Copy code
kaggle datasets download -d omkargurav/face-mask-dataset
unzip face-mask-dataset.zip -d face-mask-dataset
Train the models:

python
Copy code
python train_models.py
Evaluate the models:

python
Copy code
python evaluate_models.py
Use the trained models for prediction:

python
Copy code
python predict.py --image_path /path/to/image.jpg
Future Work
Implementing real-time detection on edge devices.
Integrating models into surveillance systems.
Handling occlusions, varying lighting conditions, and different face orientations.
Ensuring privacy and ethical use of facemask detection systems.
Extending methods to other applications such as PPE compliance in industrial settings.
Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
We would like to thank our professor for their invaluable guidance and support throughout this project. We also appreciate the assistance provided by the support staff, which was crucial in overcoming technical challenges. Finally, we extend our gratitude to our peers for their constructive feedback and collaboration.
