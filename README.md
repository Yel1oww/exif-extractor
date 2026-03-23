# Exif Extractor v1.0

**Exif Extractor** is a lightweight digital forensics tool designed to audit and extract hidden metadata (EXIF) from image files. It is specifically built for OSINT (Open Source Intelligence) and investigative purposes to reveal details like camera settings, timestamps, and geolocation data.

---

## 🚀 Features
* **Metadata Extraction**: Automatically pulls and translates EXIF tags into human-readable formats.
* **GPS Data Parsing**: Specifically isolates and formats GPS information, including coordinates and altitude if available.
* **File Info**: Provides quick summaries of image format, size, and mode.
* **Error Handling**: Built-in checks for missing metadata or file loading issues.

## 🛠️ Prerequisites
This tool requires the **Pillow** library to handle image processing.

pip install Pillow


## 📋 Usage
1. **Clone the repository** or download `exif-extractor.py`.
2. **Set your image path**: Open `exif-extractor.py` and modify the `image_path` variable to point to your target image.

   # Define the path to your image
   image_path = "your_image.png"

3. **Run the script**:

   python exif-extractor.py


## 🔍 How it Works
The script utilizes the `PIL.ExifTags` module to map numerical tag IDs to their descriptive names (e.g., converting tag `271` to `Make`). If GPS data is detected, it further unpacks the `GPSInfo` dictionary to provide granular location details.

## 👤 Author
* **Yel1oww**
* **Version**: 1.0

## ⚖️ License
This project is intended for educational and ethical investigative purposes. Please ensure you have permission to audit the images you analyze.
