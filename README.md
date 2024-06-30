# Context
As part of the Advanced AI course in the DSBA program, we were tasked with developing an innovative AI-based solution. This involved identifying a market need and proposing how AI can effectively address this need. Through this project, we aimed to leverage AI to create a practical solution that meets a real-world demand. This led to the creation of TrashDash, our AI-powered waste management system designed to enhance recycling rates and sustainability.

# TrashDash 
TrashDash is an innovative application designed to help users identify recyclable and non-recyclable objects using AI-powered image recognition. This application leverages advanced AI models to analyze images and provide detailed information about the recyclability of various objects. Additionally, it can detect available trash bins from uploaded images, making waste management more efficient and environmentally friendly.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
  - [Main Page](#main-page)
  - [Dashboard](#dashboard)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Introduction

In response to the growing waste management challenges in urban areas, we developed TrashDash as part of our Advanced I course in the DSBA program. TrashDash is an innovative AI-powered waste management solution designed to address the inefficiencies in current waste sorting systems. By leveraging advanced AI and data analytics, TrashDash analyzes images of waste items and provide instant feedback on their recyclability. Additionally, the app can detect and categorize available trash bins from images, further aiding in effective waste management. This ensures accurate waste sorting, reduced contamination, and enhanced recycling rates.

Our solution aims to tackle the pressing issue of improper waste disposal that leads to significant environmental impacts. With real-time data insights and user-friendly interfaces, TrashDash not only improves operational efficiency but also engages and educates users on sustainable waste practices. By focusing on high-impact areas like the Golden Triangle and La Défense in Paris, we aim to demonstrate the effectiveness of TrashDash in transforming urban waste management and contributing to a cleaner, more sustainable city.

## Features

- **AI-Powered Object Detection**: Upload an image of an object, and the app will detect and classify it as recyclable or non-recyclable.
- **Trash Bin Detection**: Upload an image of your trash bins, and the app will identify and categorize them for easier sorting of waste.
- **Webcam Support**: Use your webcam to capture images of objects and receive real-time feedback.
- **Interactive Dashboard**: View detailed analytics and data visualizations related to waste management.

## Training

- Yolov8 model has been trained for segmentation and object detection task on TACO Dataset
- TACO Dataset is a publicly available annotated dataset for Trash Detection. [TACO Dataset](http://tacodataset.org/)

## Installation
To install and run TrashDash Vision, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/Roshan-Velpula/TrashDash
    cd TrashDash
    ```

2. **Set up a virtual environment**:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages**:
    ```sh
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:
    Create a `.env` file in the root directory and add your OpenAI API key:
    ```sh
    OPENAI_API_KEY=your_openai_api_key
    ```

## Usage

### Main Page

1. **Upload Image**: Select the "Upload Image" option from the sidebar to upload an image of an object. The app will analyze the image and provide detailed information about its recyclability.

2. **Webcam**: Select the "Webcam" option from the sidebar to capture an image using your webcam. The app will process the image and provide recyclability information.

3. **Detect Available Bins**: Upload an image of your trash bins in the sidebar. The app will identify and categorize the bins, making it easier to sort waste.

### Dashboard

1. **Navigation**: Click on the "Go to Dashboard" button in the sidebar to navigate to the dashboard page.
2. **View Analytics**: The dashboard provides detailed analytics and data visualizations related to waste management.

### Running the Application

1. **Start the Streamlit app**:
    ```sh
    streamlit run trash.py
    ```
2. **Access the application**: Open your web browser and go to `http://localhost:8501`.

## Technologies Used

- **Python**: The core programming language used for the application.
- **Streamlit**: A framework for creating interactive web applications.
- **OpenAI API**: Used for AI-powered image recognition and classification.
- **YOLO (You Only Look Once)**: A real-time object detection system.
- **Pillow**: Python Imaging Library for image processing.

 ## Team Members
Maria Hallak (B00804339)
Nishtha Khurana (B00805298)
Joseph Panijel (B00811841)
Irene Sunny (B00798876)
Roshan Velpula (B00802760)


