# CV Project - Line Detection

## Overview
This project focuses on **image processing and computer vision techniques** to detect vertical and horizontal lines in an image. The image is first converted to grayscale, blurred for noise reduction, and then subjected to **edge detection and Hough Line Transform** for line detection.

## Features
- **Image Preprocessing:** Resize and convert the image to grayscale.
- **Blurring:** Apply a kernel-based blur to reduce noise.
- **Edge Detection:** Use Canny and Sobel filters to detect image edges.
- **Line Detection:** Implement Hough Line Transform to detect vertical and horizontal lines.

## Installation
To run this project, ensure you have the following dependencies installed:
```bash
pip install opencv-python numpy matplotlib scipy
```

## Usage
1. **Mount Google Drive (if using Colab)**
```python
from google.colab import drive
drive.mount('/content/drive')
```
2. **Load Image**
```python
img = cv2.imread('/content/drive/MyDrive/Jama masjid image processing/college.jpg')
cv2_imshow(img)
```
3. **Convert Image to Grayscale**
```python
Gimage = grayscale(image)
cv2_imshow(Gimage)
```
4. **Apply Blurring**
```python
Bimage = apply_blur(Gimage, kernel_size=3)
cv2_imshow(Bimage)
```
5. **Detect Lines using Hough Transform**
```python
line(Bimage)
line(Gimage)
```
6. **Apply Sobel Filters for Edge Detection**
```python
gradient_magnitude = sobel_filters(Bimage)
plt.imshow(gradient_magnitude, cmap='gray')
plt.axis('off')
plt.title('Edge Detected Image (Gradient Magnitude)')
plt.show()
```

## Dependencies
- **OpenCV** for image processing
- **NumPy** for matrix operations
- **Matplotlib** for visualization
- **SciPy** for convolution filters

## Results
The project successfully detects **horizontal and vertical lines** in an image by processing the grayscale image with Sobel filters and Hough Transform.

## Future Enhancements
- Improve noise reduction with advanced blurring techniques.
- Optimize Hough Transform parameters for better accuracy.
- Implement adaptive thresholding for edge detection.

---
**Author:** Syed Shareem Ahmad  
**Contact:** syed7.work@gmail.com

