# 🌿 PlantDoc - Plant Disease Detection using Deep Learning

PlantDoc is a deep learning–based web application that identifies plant diseases from leaf images. The application uses a Convolutional Neural Network (CNN) trained on a plant disease dataset and provides predictions through an interactive Streamlit interface. The project is containerized using Docker for easy deployment across different environments.

---

## Features

- Upload an image of a plant leaf
- Automatic image preprocessing
- Disease prediction using a trained CNN model
- Simple and interactive Streamlit interface
- Docker support for reproducible deployment

---

## Tech Stack

- Python
- TensorFlow / Keras
- Streamlit
- NumPy
- Pillow (PIL)
- Docker

---

## Project Structure

```
PlantDoc/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── .dockerignore
├── .gitignore
├── class_indices.json
│
├── trained_model/
│   ├── README.md
│   └── plant_disease_prediction_model.h5   (download separately)
│
└── README.md
```

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/PlantDoc.git
cd PlantDoc
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## Download the Trained Model

The trained CNN model is not included in this repository because it exceeds GitHub's file size limit.

Download the model from link given in trained_model/README.md

After downloading, place the file here:

```
trained_model/
    plant_disease_prediction_model.h5
```

---

## Running the Application

```bash
streamlit run app.py
```

Open:

```
http://localhost:8501
```

---

## Running with Docker

### Build the image

```bash
docker build -t plantdoc .
```

### Run the container

```bash
docker run -p 8501:8501 plantdoc
```

Open:

```
http://localhost:8501
```

---

## Model Pipeline

1. Upload leaf image
2. Image preprocessing
3. CNN inference
4. Predicted disease returned to the user

---

## Future Improvements

- Display prediction confidence
- Disease information and treatment suggestions
- Support multiple image uploads
- Deploy on Streamlit Community Cloud or another cloud platform
- Improve model accuracy with transfer learning

---

## Author

**Anandini Kashyap**

GitHub: https://github.com/anandini02
