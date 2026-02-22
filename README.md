
# Leaf Classification Using Convolutional Neural Networks

## 🌿 Project Overview
This project tackles the complex task of classifying plant species based on leaf images and morphological features. Using a dataset of 99 different species, this study implements multiple **Convolutional Neural Network (CNN)** architectures to automate identification, which has significant real-world applications in botany, agriculture, and environmental monitoring.

## ❓ Research Question
**Can we accurately classify 99 different plant leaf species based on morphological features and raw image data?**
The challenge lies in distinguishing subtle differences in shape, texture, and margin characteristics across a high number of classes.

## 📊 Dataset Details
* **Source:** [Kaggle Leaf Classification Challenge](https://www.kaggle.com/c/leaf-classification)
* **Images:** ~1,000 leaf images.
* **Engineered Features:** 192 features (64 margin, 64 shape, 64 texture).
* **Classes:** 99 unique species.

## 🛠️ Methodology
### 1. Exploratory Data Analysis (EDA)
Comprehensive analysis of class distributions (balanced at ~10 samples per species), feature distributions, and visual inspection of image pixel statistics.

### 2. Model Architectures
We developed and compared three CNN models with varying complexities:
* **Model 1:** Baseline CNN with standard Dropout and Max Pooling.
* **Model 2:** Tuned CNN with optimized hyperparameters and learning rate scheduling.
* **Model 3:** Advanced architecture incorporating both raw image data and engineered morphological features.

### 3. Training & Validation
* **Cross-Validation:** 5-Fold Stratified Cross-Validation to ensure model stability and generalization.
* **Regularization:** Early Stopping and Learning Rate Reduction (ReduceLROnPlateau) to prevent overfitting.

## 📈 Performance Evaluation
The models were evaluated using the following metrics:
* **Accuracy / F1-Score**
* **Multi-class ROC Curves** (AUC Analysis)
* **Precision-Recall Curves**
* **Kaggle Public/Private Score:** 1.07056 (Consistent scores indicate effective generalization).

## 🚀 Key Features
- ✅ **End-to-End Pipeline:** From data ingestion to Kaggle-ready submission files.
- ✅ **Hybrid Learning:** Use of both deep learning (CNN) and traditional feature vectors.
- ✅ **Advanced Visualization:** Detailed plots for model loss, accuracy, and ROC metrics.


### 1. Prerequisites (Installation)

Your notebook relies on several key data science and deep learning libraries. You should provide a `pip` command to install them.

**Libraries used in this file:**

* **Deep Learning:** `tensorflow`
* **Data Processing:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`
* **Image Handling:** `Pillow` (PIL)

Since notebook uses specific paths for the Kaggle dataset, you need to update the `BASE_PATH` variable to match their local directory.

### 2. Install Dependencies

Ensure you have Python 3.8+ installed, then run:

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib seaborn Pillow

```

### 3. Setup the Dataset

1. Download the dataset from the [Kaggle Leaf Classification Challenge](https://www.kaggle.com/c/leaf-classification/data).
2. Extract the files.
3. Update the `BASE_PATH` variable in the first code cell of `Leaf_Classification_CNN.ipynb` to point to your local dataset folder:
```python
BASE_PATH = 'your/local/path/to/leaf-classification'

```



### 4. Run the Analysis

Open the notebook in Jupyter or VS Code:

```bash
jupyter notebook Leaf_Classification_CNN.ipynb

```

## 📜 License

This project is licensed under the MIT License.



