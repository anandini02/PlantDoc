# 🌿 PlantDoc - Deep Learning Plant Disease Detection

PlantDoc is a deep learning–based web application that detects plant diseases from leaf images using a Convolutional Neural Network (CNN). The model is trained on a large plant disease dataset and deployed through an interactive Streamlit interface. The project is also containerized using Docker for reproducible deployment.

---

## 🚀 Features

- 🌱 Upload an image of a plant leaf
- 🤖 CNN-based disease prediction
- 🖥️ Interactive Streamlit web interface
- 🐳 Docker support for containerized deployment
- 📓 Complete training notebook included
- 🧪 Sample test images provided
- 🎥 Demo video included

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- Streamlit
- NumPy
- Pillow (PIL)
- Docker

---

## 📁 Project Structure

```
PlantDoc/
│
├── app.py
├── class_indices.json
├── Dockerfile
├── requirements.txt
├── .gitignore
├── .dockerignore
├── README.md
│
├── trained_model/
│   ├── README.md
│   └── plant_disease_prediction_model.h5 (download separately)
│
├── training_notebook/
│   └── PlantDoc_CNN.ipynb
│
├── test_images/
│   ├── test_apple_black_rot.JPG
│   ├── test_blueberry_healthy.jpg
│   └── test_potato_early_blight.jpg
│
└── demo/
    └── PlantDoc_demo.mp4
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/anandini02/PlantDoc.git
cd PlantDoc
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it.

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## 📥 Download the Trained Model

The trained CNN model is **not included** in this repository because it exceeds GitHub's file size limit.

Download it from:

trained_model/README.md

Place the downloaded model here:

```
trained_model/
    plant_disease_prediction_model.h5
```

---

## ▶️ Running the Application

```bash
streamlit run app.py
```

Then open:

```
http://localhost:8501
```

---

## 🐳 Running with Docker

Build the Docker image:

```bash
docker build -t plantdoc .
```

Run the container:

```bash
docker run -p 8501:8501 plantdoc
```

Open:

```
http://localhost:8501
```

---

## 📸 Demo

A demonstration video of the application is available in the `demo/` folder.

---

## 🧪 Sample Images

The `test_images/` folder contains sample images that can be uploaded to the application for testing.

---

## 📓 Training Notebook

The `training_notebook/PlantDoc_CNN.ipynb` notebook contains the complete workflow for:

- Dataset loading
- Data preprocessing
- CNN model training
- Model evaluation
- Saving the trained model

---

## 🔮 Future Improvements

- Display prediction confidence scores
- Show disease descriptions and treatment recommendations
- Improve model performance using transfer learning
- Deploy the application to a cloud platform

---

## 👩‍💻 Author

**Anandini Kashyap**

- GitHub: https://github.com/anandini02