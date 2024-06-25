# Image Classification using Deep Neural Networks

## Overview
This project aims to classify images of European road traffic signs using various machine learning techniques, with a focus on Convolutional Neural Networks (CNNs). The goal is to achieve accurate identification of traffic signs to enhance road safety and traffic management systems.

## Files
- **Code.ipynb**: Contains the Jupyter Notebook with the implementation of the models.
- **Summary.pdf**: Detailed report on the project, including data analysis, preprocessing, model training, evaluation, and comparison.
- **Datasets**: Contain images of European road traffic signs.

## Project Structure
1. **Data Loading**: 
   - Grayscale traffic sign images from original and collected datasets.
   - Images organized by shape and sign labels.
   - Data sourced from the German Traffic Sign Recognition Benchmark (GTSRB).

2. **Exploratory Data Analysis**:
   - Checking for duplicates.
   - Visualizing sample images.
   - Analyzing the distribution of shape and sign classes.
   - Plotting pixel intensity histograms.
   - Edge detection analysis.

3. **Data Preprocessing**:
   - Data scaling and formatting.
   - Data splitting into training, validation, and test sets.
   - Converting labels using one-hot encoding.

4. **Model Training**:
   - Various models were trained, including MLP, basic CNN, optimized CNN, and custom ResNet32-inspired neural network.
   - Techniques like batch normalization, regularization, dropout, and padding were applied to improve performance.
   - Data augmentation and edge detection were also utilized.

5. **Evaluation**:
   - Models were evaluated using accuracy, precision, recall, F1 score, and Cohen's Kappa.
   - Comparison of model performance on shape and sign classification tasks.
   - Visualizations to compare accuracies of different models.

## Results
- **Baseline Model (MLP)**: Achieved 69.48% accuracy for shape classification and 18.65% for sign classification.
- **Basic CNN**: Achieved 47.3% accuracy on validation data.
- **Optimized CNN with Batch Normalization**: Achieved 99.1% accuracy for shape and 99.47% for sign classification.
- **CNN with Data Augmentation**: Improved performance with 94.6% accuracy for shape and 85.44% for sign classification.
- **CNN with Edge Detection**: Achieved 94% accuracy for shape and 80% for sign classification.
- **Custom ResNet32-Inspired Model**: Achieved 78% accuracy for shape and 58% for sign classification on test data.

## Conclusion
The project successfully demonstrated the application of deep learning techniques for traffic sign classification. The optimized CNN model with batch normalization showed the best performance, highlighting the importance of proper preprocessing and hyperparameter tuning.

## Future Work
- Further optimization to handle class imbalances.
- Exploration of more advanced architectures and transfer learning.
- Real-time deployment and integration with traffic management systems.
