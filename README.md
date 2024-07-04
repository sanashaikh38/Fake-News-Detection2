# Fake-News-Detection

# Text Prediction Flask App

This project is a Flask web application that uses a pre-trained machine learning model to make predictions based on text input. The model is loaded from a file and predictions are served via an API endpoint.

## Features
- **CORS Enabled**: Allows cross-origin requests.
- **Model Prediction**: Accepts text input and returns a prediction.
- **Error Handling**: Includes robust error handling and logging.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.7 or higher
- `pip` (Python package installer)

### Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/sanashaikh38/Fake-News-Detection.git
    cd your-repo-name
    ```

2. **Install the required packages**


3. **Download the pre-trained model**
    - Ensure the model file (`model_pipeline.pkl`) is placed in the `model` directory.
    - If you don't have the model, you can train it using your preferred method and save it using `joblib`.

### Running the Application

1. **Start the Flask application**
    ```bash
    python app.py
    ```

2. **Access the application**
    - Open your web browser and go to `http://127.0.0.1:5000/`.

### Usage

- **Home Page**: The root URL serves an `index.html` file.
- **Prediction Endpoint**: Send a POST request to `/predict` with JSON data:
    ```json
    {
        "text": "Your input text here"
    }
    ```
    - **Example using `curl`**:
        ```bash
        curl -X POST -H "Content-Type: application/json" -d '{"text": "sample text"}' http://127.0.0.1:5000/predict
        ```

### File Structure

