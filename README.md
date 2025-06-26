# CSP-MI Python code: Common Spatial Pattern (CSP) for Motor Imagery EEG Classification.
This repository provides a manual implementation of the Common Spatial Pattern (CSP) algorithm for classifying EEG signals in motor imagery tasks. 
CSP is a spatial filtering technique widely used in BCI (Brain-Computer Interface) applications to enhance class separability by maximizing variance between different mental tasks.

✅ Note: The current implementation supports binary classification, but it can be easily extended to multi-class problems by applying pairwise CSP and combining results using strategies like one-vs-rest or one-vs-one.
# ✨ Features
-	Manual CSP filter computation (without relying on libraries like mne)
-	EEG channel covariance matrix calculation
-	Eigen decomposition for spatial filter extraction
-	Compatible with classification pipelines (e.g., LDA, SVM)
# 🔬 Application
This implementation is suitable for two-class motor imagery tasks such as:
-	Left vs Right hand imagination
-	Foot vs Tongue
This code can be simply extended for multi-class dataset
# 📦 Requirements

Before running the code, please make sure to:

**Download the dataset**

This implementation uses the **BCI Competition III - Dataset IVa**, which can be found at:

Dataset description: https://www.bbci.de/competition/iii/desc_IVa.html

Dataset download page: https://www.bbci.de/competition/iii/#data_set_iva

**The dataset consists of two parts:**
- Training – used to train the classifier
- Testing – used to evaluate the algorithm

📌 The main challenge of this competition was to evaluate the effectiveness of motor imagery classification methods on unseen data.

**Place the dataset files**

After downloading, place the .mat files (or other data formats provided) into the dataset/ folder or update the path in the code accordingly.

**Install required Python packages**
-	Python 3.x
-	numpy, scikit-learn,scipy, matplotlib (for demo)
