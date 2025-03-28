Celeb Search
Project Overview
This project aims to develop an accurate convolutional neural network (CNN) for classifying images of celebrities. The dataset, sourced from Kaggle, focuses on five celebrities: Angelina Jolie, Leonardo DiCaprio, Robert Downey Jr., Tom Cruise, and Megan Fox.

Model Development
The model was developed using TensorFlow's Keras API in Python 3, incorporating key libraries such as Kaggle, OS, Shutil, TensorFlow, Matplotlib, Numpy, Scikit-Learn, Seaborn, and Google Colab.

Data Preprocessing
Dataset Cleaning: Filtered to include only the specified celebrities.

Data Splitting: An 80-20 split was used for training and validation.

Image Resizing: All images were resized to 224x224 pixels for consistency.

Data Augmentation: Initially explored but later abandoned due to complications.

Model Architecture
The final model architecture includes:

Convolutional Layer: 64 neurons with 3x3 filters and ReLU activation.

Max Pooling Layer: 2x2 pooling to reduce spatial dimensions.

Flattening Layer: To convert the 2D feature maps into a 1D feature vector.

Dense Layers:

A dense layer with 128 neurons using ReLU activation.

A final dense layer with 5 neurons using softmax activation for classification.

Compilation and Training
Optimizer: Adam optimizer with a learning rate of 0.0001 and beta1 momentum of 0.95.

Loss Function: Sparse Categorical Cross Entropy.

Performance Metric: Accuracy was tracked during training.

Early Stopping: Implemented with a patience of 5 epochs to mitigate overfitting.

Experiments and Observations
Overfitting: Initial training over 25 epochs resulted in overfitting.

Optimizer Comparison: Stochastic Gradient Descent was tested but underperformed compared to Adam.

Model Complexity: Increasing the number of convolutional layers led to memorization rather than effective learning.

Hyperparameter Tuning: Adjusting the learning rate and beta1 momentum improved the loss curve.

Early Stopping: Effectively prevented overfitting and optimized computational resources.

Final Model Settings
Architecture: 1 convolutional layer, 1 pooling layer, 1 flattening layer, and 2 dense layers.

Optimizer: Adam with a learning rate of 0.0001 and beta1 momentum of 0.95.

Training: 80-20 train-test split, early stopping with a patience of 5 epochs, over 14 epochs.

Results: Achieved 95% accuracy with a loss of 0.4907.

Key Learnings
Data Augmentation: Although beneficial in theory, it introduced complexities that did not improve performance.

Hyperparameter Tuning: Fine-tuning the optimizer parameters was critical for smoothing the loss curve.

Early Stopping: Helped prevent overfitting while saving computational time.

Model Complexity vs. Data Size: Finding the right balance is essential to avoid memorization and ensure generalization.

Resources and References
Task 1: Numpy, Pandas, and Matplotlib assignments from provided resources.

Task 2 Repository: CelebSearch Task 2

Final Task Documentation: Final Task Document

Task 2 Submissions: Task 2 Submissions

Final Task Submissions: Final Task Submissions

