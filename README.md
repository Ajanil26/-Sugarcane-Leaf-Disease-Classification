Sugarcane Leaf Disease Classification
This project is a web application that classifies sugarcane leaf diseases using a deep learning model. It detects five disease types: Healthy, Mosaic, Red Rot, Rust, and Yellow.
Features

Upload an image of a sugarcane leaf for classification.
Predict the disease type with accuracy.
Display results with confidence scores.

Installation

Clone the repository:

bashCopygit clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

Install dependencies:

bashCopypip install -r requirements.txt

Run the Flask application:

bashCopypython app.py

Open http://127.0.0.1:5000/ in your browser.

Model Training
To train the model, run:
bashCopypython train.py
The model is trained on a dataset of labeled sugarcane leaf images covering the five different categories. The training process includes:

Data augmentation to improve model robustness
Transfer learning using a pre-trained CNN architecture
Fine-tuning for specific disease classification

Model Architecture
The classification model uses a convolutional neural network (CNN) based on a ResNet50 architecture with transfer learning. Key components include:

Pre-trained ResNet50 base
Custom classification head with dropout layers
Softmax activation for multi-class prediction

Requirements

Python 3.x
Flask
TensorFlow 2.x
NumPy
OpenCV
Pillow

Project Structure
Copy.
├── app.py              # Flask web application
├── model/              # Trained model files
├── static/             # CSS, JS, and image files
├── templates/          # HTML templates
├── train.py            # Script for model training
├── utils.py            # Utility functions
└── requirements.txt    # Project dependencies
How It Works

Users upload an image through the web interface
The image is preprocessed (resized, normalized)
The model predicts the disease class and confidence scores
Results are displayed to the user with appropriate recommendations

Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.
