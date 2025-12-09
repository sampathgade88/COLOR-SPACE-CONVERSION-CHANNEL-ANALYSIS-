# 📘 *ACV  – Color Space Conversion & Channel Analysis*

This project demonstrates *Automatic Image Loading, **Color Space Conversion, and **Channel Visualization* as part of an Advanced Computer Vision (ACV) laboratory experiment.

The script allows users to upload an image and processes it by converting between *RGB, **HSV, and **YCbCr* color spaces. It also extracts and visualizes individual channels to study their characteristics.

---

## 🚀 *Features*

### ✔ *Automatic Image Upload (Colab Compatible)*

* Detects any image in /content/
* If not found, prompts user to upload an image via Colab

### ✔ *Image Property Extraction*

Displays:

* Dimensions
* Channels
* Data type
* File size

### ✔ *Color Space Conversion*

Converts uploaded image into:

* *RGB*
* *HSV*
* *YCbCr (Y, Cr, Cb)*

### ✔ *Channel Splitting & Visualization*

The script splits each color space into channels:

| Color Space | Channels                                    |
| ----------- | ------------------------------------------- |
| *RGB*     | R, G, B                                     |
| *HSV*     | H (Hue), S (Saturation), V (Value)          |
| *YCbCr*   | Y (Luma), Cb (Blue-chroma), Cr (Red-chroma) |

Each channel is displayed as a *grayscale intensity map*.

### ✔ *Channel Reconstruction Demo*

Visualizes images using:

* Only Red
* Only Green
* Only Blue

To understand importance of each channel.

---

## 📦 *Requirements*

Install the following before running:

bash
pip install opencv-python matplotlib numpy


Runs best on *Google Colab* because of the upload UI.

---

## ▶️ *How to Run*

### Option 1 — *Google Colab*

1. Upload acv_lab1.py to Colab
2. Run the script
3. If no image exists in /content/, it will prompt you to upload one.

### Option 2 — Local System

1. Place an image in the same directory
2. Modify the file path manually
3. Run:

bash
python acv_lab1.py


---

## 📊 *Output Generated*

The program displays:

### *1. Original Image (RGB)*

### *2. RGB Channels (R, G, B)*

### *3. HSV Channels (H, S, V)*

### *4. YCbCr Channels (Y, Cb, Cr)*

Each displayed in a separate plot window.

It also prints:


Image Properties:
• Width x Height
• Channels
• Bits/channel
• File size


---

## 📘 *Color Space Interpretation*

### 🔹 *Hue (H)*

Represents the color tone.
Useful for object tracking and segmentation.

### 🔹 *Saturation (S)*

Color purity — lower means dull/grayish.

### 🔹 *Value (V)*

Brightness of the pixel.

### 🔹 *Y (Luma)*

Carries most structural information (brightness).

### 🔹 *Cb / Cr*

Color difference channels used in JPEG and video compression.

---

## 🧪 Experiment Purpose

This lab helps students understand:

* How images are represented in different color spaces
* Why computer vision uses HSV and YCbCr
* Importance of brightness vs chrominance separation
* Practical channel visualization for segmentation and detection

---

## 📁 *Project Structure*


ACV_LAB1/
│
├── acv_lab1.py         # Main program for image upload, conversion, display
└── README.md           # Project documentation


---

## 🤝 *Contributing*

Feel free to:

* Add GUI support
* Extend to LAB color space
* Include histogram comparisons
