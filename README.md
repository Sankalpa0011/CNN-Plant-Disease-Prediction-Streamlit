---

# CNN Plant Disease Prediction Streamlit App

---

This project is a Streamlit web application that predicts plant diseases using a Convolutional Neural Network (CNN) model. The application allows users to upload images of plants, and it returns the predicted disease.

## Project Structure

```
CNN Plant Disease Prediction Streamlit/
├── .venv/
├── app/
│   ├── test_images/
│   └── trained_model/
│       └── plant_disease_prediction_model.h5
├── class_indices.json
├── config.toml
├── credentials.toml
├── Dockerfile
├── main.py
├── requirements.txt
└── README.md
```

## Getting Started

### Prerequisites

- Python 3.7 or higher
- Git
- Streamlit

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Sankalpa0011/CNN-Plant-Disease-Prediction-Streamlit.git
   cd CNN-Plant-Disease-Prediction-Streamlit
   ```

2. **Create and activate a virtual environment**:

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows use: .venv\Scripts\activate
   ```

3. **Install the required packages**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up Git LFS**:

   ```bash
   git lfs install
   git lfs track "app/trained_model/plant_disease_prediction_model.h5"
   git add .gitattributes
   ```

### Usage

1. **Run the Streamlit app**:

   ```bash
   streamlit run main.py
   ```

2. **Upload an image** of a plant leaf, and the model will predict the disease.

### Deployment

The app can be deployed using Docker. Here are the steps:

1. **Build the Docker image**:

   ```bash
   docker build -t plant-disease-prediction .
   ```

2. **Run the Docker container**:

   ```bash
   docker run -p 8501:8501 plant-disease-prediction
   ```

### Model Training

If you want to train the model yourself, you can use the provided Jupyter notebook:

1. **Open the notebook**:

   ```bash
   jupyter notebook CNN_Classification_Plant_Disease_Prediction.ipynb
   ```

2. **Follow the instructions** in the notebook to train the model.

### Repository Contents

- `main.py`: The main Streamlit app script.
- `requirements.txt`: The list of Python packages required to run the app.
- `Dockerfile`: Configuration for Docker to deploy the app.
- `class_indices.json`: JSON file containing class indices for the model.
- `config.toml` and `credentials.toml`: Configuration files for the app.
- `app/test_images/`: Directory for storing test images.
- `app/trained_model/`: Directory containing the trained model.

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Acknowledgements

- The CNN model used in this project is based on MobileNet for transfer learning.
- This project was inspired by various plant disease datasets available online.

### Contact

For any questions or inquiries, please contact [Your Name](mailto:sankalpakavindu09@gmail.com).

---
