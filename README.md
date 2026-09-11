# Plant Disease Detection and Treatment Recommendation Using Deep Learning

## Official Project Identity

- College: SIDDAGANGA INSTITUTE OF TECHNOLOGY, TUMAKURU-572103
- University: Visvesvaraya Technological University, Belagavi
- Department: Department of Computer Science & Engineering
- Degree: Bachelor of Engineering (B.E.)
- Specialization: Computer Science & Engineering
- Project Title: Plant Disease Detection and Treatment Recommendation Using Deep Learning
- Academic Year: 2026-27
- Batch: Batch ID B66

## Project Team

1. JHENKAR S - 1SI23CS212
2. MOHAN GOWDA MR - 1SI23CS113
3. NANDA KUMAR - 1SI23CS119
4. LIKHITH D S - 1SI23CS099

## Project Guide

- Ms. YAMUNA H
- Assistant Professor
- Department of CSE
- Siddaganga Institute of Technology, Tumakuru-03

## Overview

This project is a Flask-based web application that uses deep learning for plant disease detection and treatment recommendation. It allows users to upload plant images, classify them using a Vision Transformer (ViT) model, and receive disease diagnosis, remedies, and preventive measures.

## Features

- Plant disease detection using HuggingFace Transformers ViT model
- Image upload support for disease analysis
- Disease description, cause, treatment, and prevention outputs
- User authentication and session-based access
- Detection history tracking per user
- Responsive web interface

## Tech Stack

- Frontend: Flask Templates, HTML, CSS, JavaScript
- Backend: Flask (Python)
- Model Inference: HuggingFace Transformers (ViT)
- Database: SQLite (Flask SQLAlchemy)
- Storage: Local temporary uploads for processing

## How It Works

1. The user uploads an image through the web interface.
2. The Flask backend stores the temporary image and passes it to the disease detection pipeline.
3. The preprocessing and feature-extraction pipeline prepares the image for inference.
4. The ViT model classifies the plant disease and returns the prediction results.
5. The application maps the result to detailed disease information and treatment guidance.
6. The output is displayed on the web page, and the top result is stored in the user history.

## Project Structure

```text
/app.py                  # Main Flask backend
/detection.py            # Disease detection pipeline
/disease_description.json # Disease information mapping
/templates/              # HTML templates
/static/                 # CSS, JS, and static assets
/temp/                   # Temporary uploaded images
/logs/app.log            # Application logging
```

## How to Run Locally

```bash
python -m venv venv
source venv/bin/activate   # or venv\Scripts\activate on Windows
pip install -r requirements.txt
python app.py
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
