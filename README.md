# Panoramic Image Generation
#### A program to create panoramas from three pictures: one central, one shifted left, and one shifted right. It uses homographies to seamlessly merge them into a single panoramic image.

---

## Description
This repository presents an attempt to create a panoramic image by stitching together three separate images: one central, one with the camera slightly shifted to the left, and one with the camera slightly shifted to the right. By utilizing homographies, we will manually select between five to ten points to use in our homography function.

If you wish to try it with your own images, using a tripod is recommended for stability. If not available, try to keep the camera as steady as possible.

## Installation
On your machine or within a Linux container/virtual machine, install the following Python libraries before running the code:

```
pip install numpy
pip install opencv-python
pip install matplotlib
```

## Usage
First, you will need to find the homographies between the pictures. In simple terms, homographies are mappings between images. For optimal results, it's suggested to use OpenCV for finding homographies; however, for the purpose of this program, we will define our own function.

After determining the homographies, you can use the `stitch_images` function if you wish to see how two images can be stitched together, or the `panoramic_image` function, which requires the three images mentioned earlier.

## License
This project is licensed under the MIT License.

---
