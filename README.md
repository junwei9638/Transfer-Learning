# AI Object Recognition Web App

## Overview

This project is a web-based application deployed on **Azure** that utilizes **AI technology** for real-time object recognition and classification. By leveraging **OpenCV.js** and a **KNN-Classifier**, the application enables users to train the model directly in the browser to identify and categorize various objects using a webcam.

## Features

- **Real-time Video Capture**: access the user's webcam for live video input.
- **Feature Extraction**: Automatically extracts features from objects presented in the video stream.
- **Interactive Classification**:
  - Train the model by recording examples of different objects.
  - Classify objects in real-time based on the trained model.
- **Customizable Labels**: Users can define new object categories and manage classification tags dynamically.

## Technology Stack

### Frontend & Logic
- **HTML5, CSS3, JavaScript**
- **OpenCV.js**: for computer vision processing.
- **KNN-Classifier**: For K-Nearest Neighbors classification logic.

### Infrastructure & Deployment
- **Docker**: Containerization of the web application.
- **Nginx**: Web server for serving static files and handling SSL.
- **Azure**: Cloud platform for hosting the application.
- **OpenSSL**: Used for generating self-signed SSL certificates for secure HTTPS connections.

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started) installed on your machine.
- A webcam connected to the computer.

### Installation

1.  **Clone the repository** (or download the source code):
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Build the Docker image**:
    ```bash
    docker build -t ai-object-recognition .
    ```

3.  **Run the Docker container**:
    ```bash
    docker run -d -p 443:443 ai-object-recognition
    ```

4.  **Access the Application**:
    Open your web browser and navigate to `https://localhost`.
    *Note: You may need to accept the self-signed certificate warning.*

## Usage

1.  **Grant Camera Permission**: Allow the browser to access your webcam when prompted.
2.  **Train the Model**:
    - Select a class/label.
    - Hold an object in front of the camera and press the "Train" (or corresponding) button to capture frames.
    - Repeat for different objects/classes.
3.  **Recognize Objects**:
    - Once trained, the system will attempt to predict the class of the object currently in the camera frame.
    - The predicted label and confidence score will be displayed on the screen.
