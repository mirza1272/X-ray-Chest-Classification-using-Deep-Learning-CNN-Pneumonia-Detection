# X-ray Chest Classification using CNN 🫁📊

This project is a Convolutional Neural Network (CNN) based image classifier that detects chest conditions (Normal, Pneumonia – viral or bacterial) from X-ray images. It uses data augmentation and keras-based training for accuracy and generalization.

---

## 🗂 Dataset Structure

<pre>
xraychest/
│
├── train/
│   ├── Normal/
│   ├── Pneumonia_bacteria/
│   └── Pneumonia_virus/
│
├── test/
│   ├── Normal/
│   ├── Pneumonia_bacteria/
│   └── Pneumonia_virus/
│
└── xraychest_cnn_model.ipynb
</pre>



---

## 🛠 Technologies Used

- Python 3
- TensorFlow / Keras
- Matplotlib
- CNN (Convolutional Neural Networks)
- ImageDataGenerator (for augmentation)

---

## 🧠 Model Architecture

- `Conv2D (32 filters)` → `MaxPool`
- `Conv2D (64 filters)` → `MaxPool`
- `Conv2D (128 filters)` → `MaxPool`
- `Flatten` → `Dense(128)` → `Dropout(0.6)`
- `Dense(3)` → `Softmax Activation`

---

## 📊 Model Performance

| Attempt | Accuracy | Overfitting |
|--------|----------|-------------|
| Try 1  | > 0.81   | Slightly overfit |
| Try 2  | 0.78     | No overfitting ✅ |
| Try 3  | 0.79     | Slightly overfit |

---

## 📈 Training Visualizations

Training and validation accuracy and loss graphs are plotted for monitoring overfitting and performance during training.

---

## ✅ Evaluation

Final model is evaluated on the test set using:

- Accuracy
- Loss

Model checkpoint and early stopping were used for better generalization.

---

## 📂 Run Notebook

The main code resides in:  
📄 **`xraychest_cnn_model.ipynb`**

Make sure to mount drive / adjust data paths accordingly.

---

## 📌 Notes

- Image size used: 96x96 for faster training.
- Used ImageDataGenerator for data augmentation.
- Model saved as `best_model.keras`.

---

## 📬 Author

Built by **Haseeb ur Rahman** as part of deep learning hands-on training.
