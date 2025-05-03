# ML_ASSIGNMENT_3

Here is a detailed and comprehensive README file that explains all the tasks and assignments in your repository. It is structured in a professional and academic tone, suitable for university submission.

---

# Machine Learning Assignments - Submission Repository

This repository contains my submission for **Machine Learning Assignment 3** as part of my university coursework. The repository includes various tasks and implementations related to machine learning concepts, including supervised and unsupervised learning techniques, dimensionality reduction, sequence modeling, and more. Below is a detailed explanation of the tasks performed in each file.

---

## Table of Contents
1. [Gaussian Process Beijing Dataset Analysis](#beijing-dataset-analysis)
2. [Image Classification with CNNs](#image-classification-with-cnns)
3. [Gaussian Processes for Regression](#gaussian-processes-for-regression)
4. [Dimensionality Reduction with PCA](#dimensionality-reduction-with-pca)
5. [Sequence Modeling with RNN & LSTM](#sequence-modeling-with-rnn--lstm)
6. [How to Run the Code](#how-to-run-the-code)
7. [Acknowledgments](#acknowledgments)

---

## Gaussian Process Beijing Dataset Analysis

**File:** `Beijing_Dataset.csv`

**Objective:**  
The `Beijing PM2.5 Dataset` was analyzed for regression tasks. This dataset is a real-world collection of air quality measurements, including PM2.5 concentrations, temperature, wind speed, and other meteorological variables.

### Tasks Performed:
1. **Data Cleaning and Preprocessing:**
   - Handled missing data by removing rows with null values in critical columns.
   - Selected key features (`TEMP`, `DEWP`) and the target variable (`PM2.5`).

2. **Feature Scaling:**
   - Applied normalization using `StandardScaler` to standardize features for Gaussian Process Regression (GPR).

3. **Gaussian Process Regression:**
   - Implemented GPR using the `RBF` kernel to predict PM2.5 concentrations.
   - Visualized predictions with 95% confidence intervals to quantify uncertainty.
   - Compared the performance of different kernels (RBF, Matern ν=1.5, and Matern ν=2.5) in terms of RMSE (Root Mean Squared Error).

4. **Experimentation with Larger Training Sets:**
   - Evaluated model performance with a smaller (200 samples) and larger (1000 samples) training set.
   - Observed the impact of training set size on uncertainty and model accuracy.

---

## Image Classification with CNNs

**Files:**
- `Harsh_Shelke_CNN.ipynb`

**Objective:**  
This assignment focuses on building and experimenting with **Convolutional Neural Networks (CNNs)** for image classification using the `CIFAR-10` dataset.

### Tasks Performed:
1. **Dataset Preprocessing:**
   - Loaded the CIFAR-10 dataset and normalized image pixel values to the range [0, 1].
   - Converted class labels to one-hot encoded format.

2. **Baseline CNN Model:**
   - Built a CNN with layers such as `Conv2D`, `MaxPooling2D`, and `Dense`.
   - Trained the model for 10 epochs and evaluated its accuracy on test data.

3. **Model Improvement:**
   - Enhanced the CNN by adding `BatchNormalization`, `Dropout`, and additional convolutional layers.
   - Experimented with hyperparameters such as filter size, number of filters, and activation functions.

4. **Advanced Techniques:**
   - Implemented data augmentation to improve generalization.
   - Replaced fully connected layers with `GlobalAveragePooling` for better efficiency.

5. **Analysis:**
   - Compared validation accuracy across different architectures.
   - Answered questions about the impact of depth, filter size, and regularization methods on model performance.

---

## Gaussian Processes for Regression

**Files:**
- `Harsh_Shelke_GP.ipynb`

**Objective:**  
This assignment applies **Gaussian Processes (GP)** for regression and uncertainty estimation using the `Beijing PM2.5 Dataset`.

### Tasks Performed:
1. **Dataset Preprocessing:**
   - Selected PM2.5 as the target variable and features such as temperature (`TEMP`) and dew point (`DEWP`).
   - Normalized features and target values for better GP performance.

2. **Gaussian Process Regression (GPR):**
   - Used the `RBF` kernel for GPR and visualized predictions with confidence intervals.
   - Experimented with additional kernels like `Matern` and analyzed their performance.

3. **Multivariate GPR:**
   - Extended GPR to handle two input features simultaneously.
   - Generated 2D surface plots of predictions and uncertainty.

4. **Performance Comparison:**
   - Compared the performance of GPR with linear regression.
   - Analyzed how uncertainty varies across the input space.

---

## Dimensionality Reduction with PCA

**Files:**
- `Harsh_Shelke_PCA.ipynb`
- `Harsh_Shelke_PCA.html`

**Objective:**  
This assignment explores **Principal Component Analysis (PCA)** and **Kernel PCA** for dimensionality reduction and image reconstruction using the `Olivetti Faces Dataset`.

### Tasks Performed:
1. **Dataset Preprocessing:**
   - Loaded the Olivetti Faces dataset, consisting of 400 grayscale images (64x64).
   - Visualized sample images from the dataset.

2. **PCA for Image Reconstruction:**
   - Reduced image dimensionality using PCA and reconstructed images from different numbers of components (10, 50, 100, 200).
   - Visualized the reconstructed images and compared them with the originals.

3. **Kernel PCA:**
   - Applied Kernel PCA with RBF, polynomial, and cosine kernels for nonlinear dimensionality reduction.
   - Reconstructed images and compared the quality with standard PCA.

4. **Analysis:**
   - Discussed the trade-offs between PCA and Kernel PCA in terms of computation and interpretability.
   - Analyzed how the reconstruction quality varies with the number of components.

---

## Sequence Modeling with RNN & LSTM

**Files:**
- `Harsh_Shelke_RNN_LSTM.ipynb`

**Objective:**  
This assignment focuses on modeling sequential data using **Recurrent Neural Networks (RNNs)** and **Long Short-Term Memory (LSTM)** networks on the `IMDb Movie Reviews Dataset`.

### Tasks Performed:
1. **Dataset Preprocessing:**
   - Processed the IMDb dataset, limiting vocabulary size to the top 10,000 words.
   - Padded sequences to a uniform length of 200 words.

2. **RNN Model:**
   - Built a simple RNN with an `Embedding` layer, `SimpleRNN`, and a `Dense` output layer.
   - Evaluated the performance of the RNN model.

3. **LSTM Model:**
   - Replaced the RNN with an LSTM layer to handle long-term dependencies.
   - Compared the performance of RNN and LSTM in terms of accuracy and overfitting.

4. **Advanced Techniques:**
   - Experimented with variations like stacked LSTM, LSTM with Dropout, and Bidirectional LSTM.
   - Analyzed the impact of these variations on validation accuracy.

5. **Analysis:**
   - Answered questions about the differences in performance between RNN and LSTM.
   - Discussed the advantages of LSTM in handling longer sequences.

---

