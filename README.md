# X-ray Chest Classification using Deep Learning 🫁📊

This project is a **Convolutional Neural Network (CNN)** based image classifier that detects chest conditions (Normal, Pneumonia – viral or bacterial) from X-ray images. It uses data augmentation and Keras-based training for accuracy and generalization.

---

## 🗂 Dataset Structure

<pre>
xraychest_cnn_model.ipynb
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
</pre>

---

## 📥 Download Dataset

Due to GitHub restrictions (file count and size limits), the dataset is uploaded separately on Google Drive.  
You can access and download the full dataset from the link below:

🔗 [Download Dataset Folder](https://drive.google.com/drive/folders/1XxjysmCAgsk6PmByo1OhzGgxpXdlUfdt?usp=sharing)

After downloading, extract or move the dataset folder into your project root so the structure matches the one shown above.

---

## 🛠 Technologies Used

- Python 3
- TensorFlow / Keras
- Matplotlib
- CNN (Convolutional Neural Networks)
- ImageDataGenerator (for augmentation)
- Google Colab

---

## 🧠 Model Architecture

- `Conv2D (32 filters)` → `MaxPool`
- `Conv2D (64 filters)` → `MaxPool`
- `Conv2D (128 filters)` → `MaxPool`
- `Flatten` → `Dense(128)` → `Dropout(0.6)`
- `Dense(3)` → `Softmax Activation`

---

## 📊 Model Performance

| Attempt | Accuracy | Overfitting       |
|--------|----------|-------------------|
| Try 1  | > 0.81   | Slightly overfit  |
| Try 2  | 0.78     | No overfitting ✅ |
| Try 3  | 0.79     | Slightly overfit  |

---

## 📈 Training Visualizations

Training and validation accuracy/loss graphs are plotted to monitor performance and overfitting during training.

---

## ✅ Evaluation

Final model is evaluated on the test set using:

- Accuracy
- Loss

Model checkpoint and early stopping were used for better generalization.

---

## 📂 Run Notebook

The full code resides in:  
📄 **`xraychest_cnn_model.ipynb`**

Make sure to mount your drive or adjust data paths if using Colab.

---

## 📌 Notes

- Image size used: `96x96` for faster training
- Used `ImageDataGenerator` for augmentation
- Final model saved as: `best_model.keras`

---

## 📬 Author

Built by **Haseeb ur Rahman** as part of Deep Learning hands-on training.
