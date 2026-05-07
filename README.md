# AuraHide
Bringing Harry Potter to life: A Computer Vision project using OpenCV to create a real-time invisibility cloak.

A "magic" invisibility effect created using **OpenCV** and **NumPy**. This project utilizes color-based segmentation and image processing to replace a specific color in a live video feed with a pre-recorded background.

---

## How it Works

The project is built on core Computer Vision principles:

1. **Background Capture:** The script captures the initial static background.
2. **Color Detection:** Converts frames to **HSV (Hue, Saturation, Value)** color space for robust color isolation.
3. **Calibrated Masking:** Uses real-time trackbars to find the perfect HSV range for your "cloak."
4. **Refining the Mask:** Applies **Median Blur** and **Dilation** to remove noise and smooth out the edges of the invisible area.
5. **Bitwise Operations:** Uses `cv2.bitwise_and` and `cv2.bitwise_or` to merge the current frame with the background.



## Features

* **Live Calibration:** Tweak HSV values on the fly with a dedicated UI window.
* **Morphological Processing:** Professional-grade noise reduction for a smoother effect.
* **Efficient Logic:** Optimized pixel manipulation using NumPy arrays.
