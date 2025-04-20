# Bone Fracture Classification Using Computer Vision
An Image Processing and Deep Learning Project | Ironhack Data Science Bootcamp

<details>
<summary>Overview</summary>

In this project, we applied computer vision techniques to classify bone X-ray images into two categories: fractured and non-fractured. The dataset contains X-rays from various body parts, providing a rich source of data for model training and testing. The main goal was to build a deep learning model capable of automatically detecting bone fractures, which has significant applications in medical diagnostics.

</details>

<details>
<summary>Objectives</summary>

- Split the dataset into training, validation, and test sets for proper model evaluation.
- Enhance the dataset using image augmentation techniques like rotation and flipping to improve model generalizability.
- Utilize a pre-trained model (MobileNetV2) with transfer learning for accurate and efficient classification.
- Measure the performance of the model using accuracy and confusion matrix.
- Provide a concise report with clear insights for presentation to stakeholders.

</details>

<details>
<summary>Dataset Information</summary>

The dataset consists of bone X-ray images labeled as either fractured or non-fractured, sourced from multiple body parts.  
**Dataset Download:** [Bone Fractures](https://drive.google.com/file/d/1WeuxOenviI1_ElW5ISED4MhvR_YFYdmB/view?usp=drive_link)

</details>

<details>
<summary>Methodology</summary>

### Data Preprocessing:
- Filtered out damaged or unreadable images using TensorFlow's utility functions.

### Model Design:
- The backbone of the model is MobileNetV2, a lightweight and efficient convolutional neural network (CNN).
- Used transfer learning by freezing the lower layers and fine-tuning the top layers to adapt the model to the fracture classification task.

### Training Procedure:
- Trained the model for 30 epochs with early stopping based on validation loss to prevent overfitting.
- The best performing model was saved as `best_model.keras` for future use.

### Evaluation:
- Model performance was evaluated using accuracy metrics, training and validation loss curves, and a confusion matrix.

</details>

<details>
<summary>Key Findings</summary>

- The model achieved a classification accuracy of 95%, demonstrating strong performance.
- Minimal errors of both Type I (false positives) and Type II (false negatives) were observed, ensuring reliable predictions.
- Transfer learning proved effective, allowing the model to perform well even with a moderately sized dataset.

</details>
