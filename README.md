# Image-Processing

## Overview
This repository covers fundamental concepts and practical algorithms for analyzing, transforming, and enhancing digital images. It is ideal for students, researchers, and developers who want to learn or apply image processing techniques using Python.

## Features & Modules

- **Automated Coin Classification and Radius Estimation:** Detect and classify coins, estimate their radii—demonstrates automated object analysis.
- **Basic Image Operations:** Core arithmetic and quantization for image enhancement.
- **Enhancement and Segmentation:** Techniques to improve image quality and segment objects.
- **Image Segmentation and Edge Detection:** Includes Canny detector and other edge-based methods.
- **Image Distance:** Methods for comparing and quantifying image similarity.
- **Morphological Operations and Object Analysis:** Erosion, dilation, opening, closing, top-hat, and more for shape manipulation and analysis.
- **Morphology Algorithms for Feature Extraction:** Extracts features using skeletonization and other advanced techniques.
- **Operator:** Filters for noise removal and smoothing (e.g., median filter).
- **Shape Feature Extraction and Classification:** Automated extraction/classification of shapes and objects.

## Folder Structure

```
├── Automated Coin Classification and Radius Estimation
├── Basic image operations
├── Enhancement and Segmentation
├── Image Segmentation and Edge Detection Techniques
├── Image distance
├── Morphological Operations and Object Analysis
├── Morphology Algorithms for Feature Extraction and Analysis
├── Operator
├── Shape Feature Extraction and Classification of Objects
├── README.md
```

## Getting Started

### Prerequisites
- Python 3.x
- numpy, opencv-python, matplotlib

### Installation
```bash
git clone https://github.com/Yahya-Sabbagh/Image-Processing.git
cd Image-Processing
pip install numpy opencv-python matplotlib
```

### Usage Example

**Morphological Skeletonization:**
```python
import cv2
from skimage.morphology import skeletonize
import numpy as np

img = cv2.imread('binary_image.png', 0)
binary = img // 255
skeleton = skeletonize(binary)
cv2.imwrite('skeleton.png', skeleton * 255)
```

**Canny Edge Detection:**
```python
import cv2
img = cv2.imread('input.jpg', 0)
edges = cv2.Canny(img, 100, 200)
cv2.imwrite('edges.jpg', edges)
```

## Contribution

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

See `CONTRIBUTING.md` for more.

## License
This project is licensed under the MIT License.

## Credits
Created by Yahya Sabbagh. Thanks to all contributors and the open-source community.
