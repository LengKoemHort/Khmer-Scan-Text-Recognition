

# Khmer Scene-Text Recognition (KSTR)

This repository contains the implementation of the Khmer Scene-Text Recognition (KSTR) project, an end-to-end pipeline for detecting and recognizing Khmer text in real-world images. The project integrates **YOLOv8** for text detection and **TrOCR** for text recognition, achieving a Character Error Rate (CER) of 0.129 and Word Error Rate (WER) of 0.375 on the expanded KhmerST dataset. This work supports applications like digital archiving and automated navigation in Cambodia.

## Project Overview

The KSTR project expands the KhmerST dataset from 1544 to 2551 images, including 1007 Google Maps images, resulting in 11,351 annotated text regions. The pipeline processes full images by:
- Detecting text regions using YOLOv8 (mAP@0.5: 0.586).
- Recognizing text in cropped regions using TrOCR, fine-tuned for Khmer script.
- Supporting real-world Khmer OCR applications.

The project was developed as part of the Project Practicum for graduation at the Royal University of Phnom Penh.

## Features
- **Text Detection**: Uses YOLOv8 to identify text regions in images.
- **Text Recognition**: Employs TrOCR for accurate Khmer text recognition.
- **Dataset**: Expanded KhmerST dataset with 2551 images and 11,351 text regions.
- **Applications**: Enables digital archiving, automated translation, and navigation in Cambodia.

## Requirements
To run this project, install the following dependencies:
```bash
pip install torch torchvision opencv-python matplotlib ultralytics transformers huggingface_hub pillow
