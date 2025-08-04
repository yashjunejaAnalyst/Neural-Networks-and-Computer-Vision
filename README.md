# Neural-Networks-and-Computer-Vision

**Project Title:**
HelmNet: A Deep Learning-Based Helmet Detection System for Workplace Safety

**Project Objective:**
To develop a deep learning image classification model that automatically detects whether a worker in an image is wearing a safety helmet or not wearing a safety helmet, enhancing workplace safety enforcement and minimizing risks due to human error in surveillance.

Project Approach:

1.) Data Collection & Preprocessing:
Dataset: 631 labeled images (311 with helmet, 320 without).
Diverse backgrounds like construction sites and factories.
Preprocessing included image resizing, Gaussian blurring, and train-validation splitting.

2.) Model Development:

Model 1: VGG-16 base model.
Model 2: VGG-16 + Feed Forward Neural Network (FFNN).
Model 3: VGG-16 + FFNN + Data Augmentation.
Evaluated using accuracy, confusion matrix, and performance metrics.

3.) Performance Evaluation:

Compared train vs. validation accuracy.
Analyzed false negatives (missed helmet violations).
Data augmentation did not yield better results due to already diverse dataset.

4.) Model Selection:

Final model: VGG-16 + FFNN, offering a better trade-off between accuracy and complexity.

**Outcome:**

1.) Model Accuracy: ~61–62% on validation set, with higher training accuracy, indicating slight overfitting.

2.) Business Insight: Automated detection is feasible and can assist in real-world deployment.

3.) Key Risk Identified: False negatives (workers without helmets misclassified) pose safety concerns.

**Recommendations:**

* Deploy in a controlled pilot setting.

* Retrain model with class weighting to penalize false negatives.

* Expand dataset with edge cases and varied lighting conditions.

* Integrate real-time alerts for safety workflow enhancement.

* Explore advanced models (e.g., YOLOv5, EfficientNet) for future scalability.
