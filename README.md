# Image to Excel Converter (OCR & AI Powered)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Tesseract](https://img.shields.io/badge/OCR-Tesseract_5-green.svg)
![Status](https://img.shields.io/badge/Status-Maintained-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-orange.svg)

## 📄 Overview
**Image to Excel Converter** is a robust Python automation tool designed for Data Analysts and ML Engineers. It leverages **Computer Vision** and **Optical Character Recognition (OCR)** to extract tabular data from images (JPG, PNG) and convert them into structured Excel spreadsheets (`.xlsx`).

Unlike simple OCR tools, this project utilizes `img2table` and `Tesseract` to preserve the **structural integrity** of tables, including rows, columns, and headers.

---

## ✨ Key Features
* **Intelligent Table Detection:** Automatically detects table borders and cells using Computer Vision algorithms.
* **Multi-Table Support:** Extracts multiple tables from a single image and saves them into separate Excel sheets.
* **OCR Integration:** Built on top of **Tesseract 5** (LSTM neural networks) for high-accuracy text recognition.
* **Borderless Table Handling:** Capable of detecting implicit rows/columns even without visible grid lines.
* **Automated Formatting:** Outputs clean, readable Excel files compatible with Pandas analysis.

---

## 🛠️ Architecture & Tech Stack
* **Language:** Python 3.x
* **Core Engine:** `img2table` (Table detection logic)
* **OCR Engine:** `Tesseract-OCR` (Google's LSTM-based OCR engine)
* **Data Processing:** `Pandas` & `OpenPyxl`
* **Image Processing:** `OpenCV` & `Pillow`

---

## 🚀 Installation & Setup

### 1. System Dependencies (Tesseract OCR)
This project requires Tesseract engine installed on your OS.

* **Windows:** Download the installer from [UB-Mannheim/tesseract](https://github.com/UB-Mannheim/tesseract/wiki).
    * *Note:* Add the installation path to your System Environment Variables or configure it in the script.
* **Linux (Ubuntu/Debian):**
    ```bash
    sudo apt update
    sudo apt install tesseract-ocr libtesseract-dev
    ```

### 2. Python Libraries
Clone the repository and install the required packages:

```bash
git clone [https://github.com/YourUsername/Image-to-Excel-OCR.git](https://github.com/YourUsername/Image-to-Excel-OCR.git)
cd Image-to-Excel-OCR
pip install -r requirements.txt
