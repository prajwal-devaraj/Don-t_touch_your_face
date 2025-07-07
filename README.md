# Don't Touch Your Face – Deep Learning Detection System

This project is designed to detect whether a person is touching their face using deep learning and computer vision. The goal is to encourage better hygiene by identifying and alerting users when face-touching behavior is detected. This is especially useful in public health scenarios such as during the COVID-19 pandemic.

## Project Overview

The system includes two main components:

- Model training using labeled image data of face-touching and non-face-touching.
- Real-time detection using webcam feed and a trained model.

## Files and Descriptions

- `ModelTrainingCode.ipynb`: Jupyter Notebook used to train a Convolutional Neural Network (CNN) model to distinguish between face-touching and no-face-touching.
- `Testing(Don’t_Touch_Your_Face).ipynb`: Jupyter Notebook used to test the trained model on real-time webcam feed or video input.
- `dataset/`: Folder containing training data divided into `touch/` and `no_touch/` subfolders.
- `model/`: Optional folder to store trained models in `.h5` or `.pkl` format.

## Features

- Trains a CNN-based classification model.
- Supports binary classification: face-touch vs no-touch.
- Real-time detection via webcam using OpenCV.
- Easily expandable for more classes or more complex behavior recognition.

## Technologies Used

- Python 3.x
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook

## Installation

1. Clone the repository:

git clone https://github.com/yourusername/dont-touch-your-face.git
cd dont-touch-your-face

2. Install the dependencies:

pip install tensorflow opencv-python numpy matplotlib

Or create a `requirements.txt` file and run:

pip install -r requirements.txt


## Dataset Structure

Organize your dataset as follows:

dataset/
├── touch/
│ ├── image001.jpg
│ └── ...
└── no_touch/
├── image001.jpg
└── ...

Ensure images are preprocessed to a consistent size and format for effective model training.

## How to Run

### Train the Model

1. Open `ModelTrainingCode.ipynb` in Jupyter Notebook.
2. Configure dataset path and image size.
3. Run the notebook to:
   - Load and preprocess data
   - Define and compile the CNN model
   - Train the model
   - Save the model to disk

### Test the Model

1. Open `Testing(Don’t_Touch_Your_Face).ipynb`.
2. Load the saved model.
3. Use OpenCV to capture video frames.
4. Perform predictions on live webcam data.
5. Display real-time feedback based on prediction.

## Sample Output

Screenshots or video demonstrations showing correct classification (touch vs no-touch) can be added here for reference.

## Future Improvements

- Improve accuracy with a larger dataset.
- Integrate sound or vibration alerts for detected face-touching.
- Deploy on mobile or embedded devices using TensorFlow Lite.
- Use hand and face landmark detection for better precision.

## Authors

- Prajwal Devaraj
- (Add additional contributors here if applicable)

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgments

- Built as a project to promote personal hygiene and behavioral awareness.
- Thanks to open-source communities for tools and datasets.
