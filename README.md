This repository contains a Jupyter Notebook (`AI-Powered Image Recognition Web App.ipynb`) that guides you through building a simple **AI-Powered Image Recognition Web Application** using **Flask** and a pre-trained **Keras** model.

## Project Overview

This notebook provides the foundational code and steps to deploy a machine learning model (e.g., for dog/cat classification) as a web application. It covers everything from setting up a Flask server to handling image uploads, preprocessing them, making predictions, and displaying results through a web interface.

## Key Highlights

  * **Flask Web Framework**: Learn how to create a basic web application to serve your AI model.
  * **Keras Model Integration**: Integrate a pre-trained deep learning model (`dog_vs_cat.h5` suggested by the code).
  * **Image Preprocessing**: Implement functions to prepare uploaded images for model inference.
  * **Prediction Endpoints**: Set up routes to handle image uploads and return prediction results.
  * **User Interface**: Includes a basic HTML template for image submission.

## Getting Started

### Prerequisites

To run this project, you will need Python and the following libraries:

  * `flask`
  * `tensorflow` (which includes Keras)
  * `opencv-python`
  * `numpy`

You can install them using pip:

```bash
pip install flask tensorflow opencv-python numpy
```

### How to Run

1.  Ensure you have your trained Keras model saved as `dog_vs_cat.h5` in the appropriate directory (or modify the code to point to your model).

2.  Save the code from the notebook into a Python file (e.g., `app.py`) within a new directory for your Flask app. Create a `templates` folder in the same directory and save the HTML content as `index.html` inside it.

3.  Navigate to your app folder in the terminal.

4.  Run the Flask application:

    **On Linux/macOS:**

    ```bash
    export FLASK_APP=app.py
    flask run
    ```

    **On Windows:**

    ```bash
    set FLASK_APP=app.py
    flask run
    ```

5.  Open your web browser and navigate to `http://127.0.0.1:5000/` to interact with the application and upload images for recognition.
