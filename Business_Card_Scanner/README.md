# Business Card Scanner

## Description

This project aims to provide a tool for scanning business cards using computer vision and optical character recognition (OCR) techniques. The goal is to extract relevant information such as name, company, job title, phone number, email address, and website from an image of a business card.

*(Add more specific details about your project's approach or unique features here.)*

## Features

*   Loads an image of a business card.
*   Preprocesses the image to enhance text clarity (e.g., grayscale conversion, thresholding, noise reduction).
*   Utilizes an OCR engine (like Tesseract) to extract text from the image.
*   Parses the extracted text to identify and categorize contact information (Name, Title, Company, Phone, Email, Website, Address).
*   Outputs the extracted information in a structured format (e.g., console print, JSON, CSV).

*(Adjust this list based on the actual features implemented in your script.)*

## Dependencies

This script relies on the following Python libraries:

*   **OpenCV (`opencv-python`)**: For image loading, preprocessing, and potentially contour detection.
*   **Pytesseract (`pytesseract`)**: Python wrapper for Google's Tesseract-OCR Engine.
*   **Tesseract OCR Engine**: Needs to be installed separately on your system. Follow instructions for your OS: Tesseract Installation Guide
*   **NumPy (`numpy`)**: For numerical operations, often used with OpenCV.
*   **(Optional) Regular Expressions (`re`)**: For pattern matching during text parsing.
*   **(Optional) Matplotlib (`matplotlib`)**: For displaying images during development or debugging.

*(Modify this list based on the actual libraries your `Business_Card_Scanner.py` uses.)*

## Installation

1.  **Clone the repository (if applicable):**
    ```bash
    git clone <your-repository-url>
    cd <repository-directory>
    ```
2.  **Install Tesseract OCR:**
    *   Follow the official installation guide for your operating system: https://github.com/tesseract-ocr/tesseract#installing-tesseract
    *   Make sure the `tesseract` command is added to your system's PATH or configure the path within the script if needed.
3.  **Install Python dependencies:**
    ```bash
    pip install opencv-python pytesseract numpy matplotlib
    ```
    *(Add/remove packages as needed based on your `Dependencies` section.)*

## Usage

1.  Place the business card image file you want to scan in a known directory.
2.  Run the script from your terminal:

    ```bash
    python Business_Card_Scanner.py --image path/to/your/business_card.jpg
    ```
    *(Adjust the command-line arguments (`--image` in this example) based on how your script accepts input.)*

3.  The script will process the image and output the extracted contact information to the console (or save it to a file, depending on your implementation).

**Example:**

```bash
python Business_Card_Scanner.py --image sample_cards/card1.png
