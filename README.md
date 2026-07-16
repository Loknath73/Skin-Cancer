# 🩺 Skin Cancer (Melanoma) Detection using CNN

A deep learning project that classifies dermoscopic skin lesion images as **Benign** or **Malignant (Melanoma)** using **Transfer Learning**. The model is built with **TensorFlow/Keras** and utilizes the pretrained **MobileNetV2** architecture to achieve efficient and accurate skin cancer detection.

---

## 🚀 Tech Stack

* **Programming Language:** Python
* **Deep Learning Framework:** TensorFlow / Keras
* **Model Architecture:** MobileNetV2 (Transfer Learning)
* **Image Processing:** OpenCV, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Model Evaluation:** Scikit-learn

---

## 📊 Dataset & Train-Test Split

| Item                  | Details                                                    |
| --------------------- | ---------------------------------------------------------- |
| Classes               | Benign, Malignant                                          |
| Total Training Images | 7,684                                                      |
| Validation Split      | **20% (1,921 images)**                                     |
| Test Images           | **1,000 (500 Benign, 500 Malignant)**                      |
| Image Size            | **224 × 224 pixels**                                       |
| Normalization         | `rescale = 1./255`                                         |
| Data Augmentation     | Rotation, Width/Height Shift, Shear, Zoom, Horizontal Flip |

---

## 🧠 Model

* **Base Model:** MobileNetV2 (Pretrained on ImageNet)
* **Transfer Learning:** Frozen pretrained layers with a custom classification head
* **Task:** Binary Image Classification (Benign vs. Malignant)
* **Loss Function:** Binary Crossentropy
* **Optimizer:** Adam
* **Output Activation:** Sigmoid

---

## 📈 Results

* ✅ High accuracy for melanoma classification.
* ✅ Transfer learning improves performance with limited medical image data.
* ✅ Data augmentation enhances model generalization and reduces overfitting.
* ✅ Lightweight MobileNetV2 enables fast and efficient inference.

---

## ▶️ Installation

Install the required dependencies:

```bash
pip install tensorflow keras numpy matplotlib seaborn scikit-learn opencv-python
```

---

## ▶️ Run the Project

Train the model:

```bash
python train.py
```

Run inference:

```bash
python predict.py
```

---

## 📂 Output Files

After training, the following files are generated:

* `mobilenetv2_skin_cancer_model.h5`
* `training_history.pkl`

---

## 👨‍💻 Author

**Loknath Basak Anup**
B.Sc. in Computer Science & Engineering
United International University (UIU)



