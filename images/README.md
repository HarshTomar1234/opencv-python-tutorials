# Sample Images for OpenCV Tutorials

This directory contains sample images used throughout the OpenCV tutorials. Using these shared images ensures consistency across examples and makes it easier for users to follow along.

## Image Sources

- `lena.jpg` - The classic Lena test image, widely used in image processing
- `opencv_logo.png` - The official OpenCV logo
- `shapes.jpg` - A simple image with various geometric shapes
- `chessboard.jpg` - A chessboard pattern useful for camera calibration
- `faces.jpg` - Sample image with faces for face detection
- `road.jpg` - Road scene for lane detection examples
- `text.jpg` - Image with text for OCR examples
- `noise.jpg` - Image with various types of noise for filtering examples
- `panorama_1.jpg` and `panorama_2.jpg` - Overlapping images for stitching examples

## Usage

When using these images in the tutorial scripts, use relative paths like:

```python
import cv2
import os

# Get the path to the images directory relative to the script
script_dir = os.path.dirname(os.path.abspath(__file__))
images_dir = os.path.join(os.path.dirname(script_dir), 'images')

# Load an image
img = cv2.imread(os.path.join(images_dir, 'lena.jpg'))
```

This ensures that the scripts can find the images regardless of which directory they're run from.

## License Information

The images in this directory are either created specifically for these tutorials, in the public domain, or used under appropriate licenses. If you plan to use these images outside of these tutorials, please check the original sources for license information.