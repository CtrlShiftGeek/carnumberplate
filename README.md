# 🚗 Car Number Plate Detection using EasyOCR

This project detects vehicle number plates in images or video streams and extracts the text using EasyOCR. It combines OpenCV for image processing and EasyOCR for optical character recognition (OCR), supporting various languages including English and regional formats.

---

## 🧠 Features

- Detects and extracts number plates from static images or webcam feed.
- Recognizes plate text using EasyOCR.
- Outputs processed images with bounding boxes and recognized text.
- Lightweight and easy to set up.

---

## 🗂️ Project Structure

```
car-number-plate-detection/
│
├── images/                 # Input images
├── output/                 # Output images with results
├── number_plate_ocr.py     # Main detection and OCR script
├── requirements.txt        # List of dependencies
└── README.md               # Project documentation
```

---

## 🔧 Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/car-number-plate-detection.git
cd car-number-plate-detection
```

### 2. Create and activate a virtual environment (optional)

```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

If you don’t have a `requirements.txt` yet, here are the core packages you'll need:

```bash
pip install easyocr opencv-python
```

> Note: EasyOCR will also install PyTorch automatically.

---

## 🚀 Usage

### Detect and extract from an image

```bash
python number_plate_ocr.py --image images/car.jpg
```

### Live detection using webcam (optional)

```bash
python number_plate_ocr.py --webcam
```

---

## 🔍 Sample Output

- Text from license plate is printed in the terminal.
- Processed image saved in the `output/` directory with bounding boxes and recognized text.

---

## 🧰 Technologies Used

- Python 3
- OpenCV (image processing and plate detection)
- EasyOCR (text recognition)
- Numpy

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ✨ Acknowledgements

- [OpenCV](https://opencv.org/) for computer vision tools.
- [EasyOCR](https://github.com/JaidedAI/EasyOCR) for multilingual OCR.
- Pretrained Haar cascades or YOLO models for plate detection (optional).
