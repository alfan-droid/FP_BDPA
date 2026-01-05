# Sleep Disorder Classification using Deep Learning

![Python](https://img.shields.io/badge/Python-3.10-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange)
![Keras](https://img.shields.io/badge/Keras-Sequential-red)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Project Overview
This project is a Final Project for the **Advanced Artificial Intelligence** course. We implemented a **Deep Learning model (Sequential Neural Network)** to classify sleep disorders based on lifestyle and health metrics.

The model predicts whether a person belongs to one of three categories:
1. **None** (Healthy/No Disorder)
2. **Insomnia**
3. **Sleep Apnea**

Using a dataset containing physical activity, stress levels, and sleep duration, our model achieved an accuracy of **~90%**.

## 👥 Team Members (Kelompok 1)
| Student ID | Name | University | Role |
| :--- | :--- | :--- | :--- |
| **23.11.5438** | Alfan Shobron Jamal | Univ. Amikom | Model Training & Code Dev |
| **23.11.5822** | Awaludin | Univ. Amikom | Data Preprocessing & Tuning |
| **2303010120** | Ariel Ivan Al-Hakim | Univ. Perjuangan | Report & Presentation |
| **2303010104** | Ravindra Diaz Abigail | Univ. Perjuangan | Evaluation & Documentation |

## 📂 Dataset
We used the **Sleep Health and Lifestyle Dataset** from Kaggle.
* **Size:** 374 rows, 13 columns.
* **Features:** Gender, Age, Occupation, Sleep Duration, Quality of Sleep, Physical Activity Level, Stress Level, BMI Category, Blood Pressure, Heart Rate, Daily Steps.
* **Target:** `Sleep Disorder` (Multi-class classification).

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:**
    * `TensorFlow / Keras` (Model Architecture)
    * `Pandas & NumPy` (Data Manipulation)
    * `Scikit-learn` (Preprocessing & Evaluation)
    * `Matplotlib & Seaborn` (Visualization)
* **Environment:** Google Colab / Jupyter Notebook

## 🧠 Model Architecture
We utilized a **Sequential Artificial Neural Network (ANN)**:
1.  **Input Layer:** 11 Features (Preprocessed & Scaled).
2.  **Hidden Layer 1:** Dense (64 neurons, ReLU activation).
3.  **Dropout Layer:** Rate 0.3 (to prevent overfitting).
4.  **Hidden Layer 2:** Dense (32 neurons, ReLU activation).
5.  **Output Layer:** Dense (3 neurons, Softmax activation).

## 📊 Results
The model was evaluated on unseen test data (20% split).

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **90%** |
| **Precision (Macro)** | 0.88 |
| **Recall (Macro)** | 0.87 |
| **F1-Score (Macro)** | 0.87 |

**Detailed Class Performance:**
* **Healthy:** High precision (95%), minimal false positives.
* **Insomnia vs. Apnea:** The model effectively distinguishes between these two disorders with F1-scores > 0.80.

## 🚀 How to Run
1.  Clone this repository:
    ```bash
    git clone [https://github.com/username/repo-name.git](https://github.com/username/repo-name.git)
    ```
2.  Install required libraries:
    ```bash
    pip install pandas numpy tensorflow scikit-learn matplotlib
    ```
3.  Open the notebook `Sleep_Disorder_Prediction.ipynb` in Jupyter or Google Colab.
4.  Run all cells to see the preprocessing, training, and evaluation steps.

## 🔗 Links
* **Source Code (Gist):** [View Code Here](https://gist.github.com/ravindradiaz/1edf4a5922cedea11bce4b7d8c6be26f)
* **Dataset Source:** [Kaggle - Sleep Health and Lifestyle](https://www.kaggle.com/)

---
*Created for Final Project AI Lanjut 2026.*
