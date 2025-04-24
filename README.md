
# 🖋️ Signature Matching System

A Python-based Signature Matching System that detects and verifies the authenticity of handwritten signatures using image processing and a neural network classifier. The system classifies signatures as **genuine** or **forged**, making it useful in legal, financial, and administrative applications.

## 🚀 Features

- ✅ Verify whether a signature is genuine or forged
- 🖼️ Image preprocessing (grayscale, binarization, resizing, thinning)
- 🔍 Feature extraction from signature images
- 🧠 Trainable Multilayer Perceptron (MLP) model using TensorFlow v1
- 📊 Accuracy and prediction results displayed in terminal
- 🗃️ Data saved and processed in CSV format

---

## 📂 Project Structure

```
Signature_matching_system/
├── dataset/                   # Folder containing genuine & forged signature images
├── Features/                  # CSV files for training and testing
├── Model/                     # Saved MLP model
├── __pycache__/
├── feature_extraction.py      # Extracts features from signature images
├── image_preprocessing.py     # Preprocesses images for feature extraction
├── train_mlp_model.py         # Trains MLP model
├── test_signature.py          # Tests new signatures
├── utils.py                   # Utility functions
└── README.md
```

---

## 🧰 Technologies Used

- Python
- OpenCV
- NumPy & Pandas
- TensorFlow v1
- Matplotlib (for visualization)

---

## ⚙️ Installation & Setup

1. **Clone the repository**

```bash
git clone https://github.com/KeerthanaD4/Signature_matching_system.git
cd Signature_matching_system
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

> *If `requirements.txt` is missing, install manually:*
```bash
pip install opencv-python tensorflow==1.15 numpy pandas matplotlib
```

3. **Run feature extraction**

```bash
python feature_extraction.py
```

4. **Train the MLP model**

```bash
python train_mlp_model.py
```

5. **Test with a new signature**

```bash
python test_signature.py
```

---

## 📊 Dataset

The project expects a dataset folder structured like:

```
dataset/
├── genuine/
│   ├── user1_01.png
│   ├── user1_02.png
│   └── ...
└── forged/
    ├── user1_01.png
    ├── user1_02.png
    └── ...
```

Make sure the dataset images are pre-labeled as `genuine` or `forged`.

---

## 🤖 Model

The neural network is a **Multilayer Perceptron (MLP)** that takes in extracted features and classifies the signature as either **genuine** (1) or **forged** (0). Training results and saved models are stored under the `Model/` directory.

---

## 📌 Future Improvements

- Switch to TensorFlow 2.x and Keras for improved model development
- Integrate CNNs for automatic feature extraction
- Develop a GUI using Flask or Streamlit
- Add support for more signature datasets

---

## 📬 Contact

Maintained by [KeerthanaD4](https://github.com/KeerthanaD4)  
Feel free to open issues or submit pull requests!

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
