## Overview

This is a Python-based web application that allows users to upload images and extract text from them using Optical Character Recognition (OCR). The application leverages the power of **Tesseract OCR** via the `pytesseract` library, along with OpenCV (`cv2`), NumPy, and PIL for image processing. The web interface is built using **Flask**.

## Features

- Extract text from various image formats (JPEG, PNG, etc.)
- Preprocess images to improve text detection
- Simple web interface for image upload and text extraction
- Support for multiple languages (configurable through Tesseract)

## Technologies Used

- **Python 3.9+**
- **Flask** - A micro web framework for Python
- **Pytesseract** - Python wrapper for Google's Tesseract OCR
- **OpenCV (cv2)** - Image processing library
- **NumPy** - Numerical computations library for image manipulation
- **Pillow (PIL)** - Python Imaging Library for working with images

## Prerequisites

Before you begin, ensure you have met the following requirements:

- **Python 3.9+** installed
- **Tesseract OCR** installed on your machine. Follow the installation guide [here](https://github.com/tesseract-ocr/tesseract).

## Usage

1. Open the web interface.
2. Upload an image from your local machine.
3. Click on **Extract Text**.
4. The extracted text will be displayed on the web page.

## Code Structure

```bash
.
├── app.py                # Main application script
├── static/
│   ├── css/
│   └── img/
├── templates/
│   ├── index.html        # Main webpage
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

### Core Libraries & Functionality

- **Flask**: Handles web server functionality and routes.
- **Pytesseract**: Interacts with Tesseract OCR to perform text extraction.
- **OpenCV (cv2)**: Preprocesses images (e.g., resizing, grayscale, thresholding).
- **Pillow**: Handles image input/output operations.
- **NumPy**: Supports array manipulation and image processing tasks.

### Image Preprocessing

Before text extraction, the application preprocesses images for better OCR results. This includes:

- **Grayscale conversion**
- **Noise removal**
- **Thresholding**

These processes help Tesseract identify text more accurately.


## Troubleshooting

- **Tesseract not found**: Ensure Tesseract is installed and accessible in your system's PATH.
- **Poor OCR results**: Try different image preprocessing methods, such as binarization, resizing, or contrast enhancement.
- **Slow processing**: Large images may take longer to process. Consider resizing or downscaling images before passing them to the OCR engine.

## Contributing

Contributions are welcome! Please submit pull requests or issues to improve the project.

### Steps to Contribute:

1. Fork the project
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Open a pull request

