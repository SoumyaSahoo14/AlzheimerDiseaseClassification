# 🧠 Alzheimer's Disease MRI Classifier

This project uses deep learning models to classify brain MRI images into four categories of Alzheimer's disease progression:

- **NonDemented**
- **VeryMildDemented**
- **MildDemented**
- **ModerateDemented**

We experimented with **ResNet50**, **VGG19**, and **InceptionV3** architectures. Among these, **ResNet50 achieved the best accuracy** and was integrated into the Streamlit web app for final deployment.

---

## 📂 Project Structure

```
.
├── alzheimer_resnet50.ipynb        # Jupyter notebook for model training & evaluation
├── test.ipynb                      # Testing notebook for inference and comparison
├── app.py                          # Streamlit web app for deployment
└── README.md                       # Project documentation
```

---

## 🚀 Getting Started

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

> Create `requirements.txt` containing:
```txt
streamlit
tensorflow
pillow
numpy
```

### 2. Add your trained model
Make sure to place your `alzheimer_resnet50_model.h5` file in the same directory as `app.py`.

---

## 🧪 Running the Web App

To launch the Streamlit app locally:

```bash
streamlit run app.py
```

Then open your browser and navigate to the local URL .

---

## 🖼️ Sample Output

- Upload an MRI image in `.jpg`, `.jpeg`, or `.png` format.
- The app will display the predicted class along with confidence scores for all four categories.

---

## 🧠 Model Overview

- **Architectures Used**: ResNet50, VGG19, InceptionV3
- **Best Performer**: ResNet50
- **Input Size**: 176x176 pixels
- **Output Classes**: 4 (Multi-class classification)
- **Preprocessing**: Resizing, Normalization
- **Loss Function**: Categorical Crossentropy
- **Optimizer**: Adam

---

## 📦 Dataset

The MRI image dataset used in this project is publicly available on Kaggle.

👉 [Download the dataset from Kaggle](https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset)

---

## 🧾 License

This project is for academic and research use only.
