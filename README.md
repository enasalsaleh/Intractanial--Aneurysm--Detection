# Intracranial Aneurysm Detection

This project presents an artificial intelligence–based system for the automated detection of intracranial aneurysms using brain computed tomography (CT) images. Intracranial aneurysms are abnormal dilations of cerebral blood vessels that may lead to life-threatening complications such as hemorrhage or stroke if not detected early. The aim of this project is to develop a reliable deep learning model that assists in identifying aneurysm cases accurately and efficiently.

The dataset used in this project is the “Computed Tomography (CT) of the Brain” dataset obtained from Kaggle. It contains brain CT images provided in JPG and DICOM formats, covering multiple brain conditions. For the purpose of this study, the dataset was reorganized into a binary classification problem consisting of two classes: aneurysm and non-aneurysm.

Several preprocessing steps were applied to ensure data consistency and improve model performance. These steps include resizing all images to a fixed resolution of 224×224 pixels, normalizing pixel values, converting medical image formats when necessary, and preparing the data for deep learning input. To reduce overfitting and enhance generalization, data augmentation techniques such as rotation, flipping, zooming, and brightness adjustment were applied to the training dataset.

The core of the system is based on the Xception deep learning architecture, which is a convolutional neural network that utilizes depthwise separable convolutions for efficient and powerful feature extraction. Transfer learning was applied by initializing the model with pretrained weights and fine-tuning it for the binary classification task. This approach allows the model to learn complex and subtle patterns associated with aneurysms while maintaining computational efficiency.

The model was trained and evaluated using separate training, validation, and testing datasets. Performance evaluation was conducted using accuracy metrics and confusion matrix analysis. The experimental results demonstrate strong classification performance, achieving high accuracy across training, validation, and testing phases, which confirms the effectiveness of deep learning for medical image analysis.

This project highlights the potential of artificial intelligence as a supportive diagnostic tool in healthcare. The proposed system does not replace clinical expertise but can assist clinicians by providing fast and consistent predictions, supporting early detection of intracranial aneurysms and improving diagnostic reliability.

---

## Project Files
- Xception_exp.ipynb : Google Colab notebook containing the code.
- ct_model.h5 : Trained deep learning model.
- extra test/ : Folder containing sample images used to test the model.

---

## How to Run (Google Colab)
1. Open Google Colab.
2. Upload the file Xception_exp.ipynb.
3. Upload the trained model file ct_model.h5.
4. Upload the test images folder (`extra test`) when prompted.
5. Run all cells in order to execute the project and test the model on the images.

---
#Note: The trained model file (ct_model.h5) is not included in the repository due to GitHub file size limitations.
