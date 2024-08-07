# Image_Scaling_and_Rotation

# Experiment 1

## Objective:

To develop a Python program that reads an image and performs image scaling and rotation
using custom-implemented functions.

# Image Processing with OpenCV

This repository contains Python code for performing image processing operations such as scaling and rotating images using nearest neighbor and bilinear interpolation methods. The operations are performed using the OpenCV library.

## Requirements

To run the code, you need to have the following libraries installed:
- OpenCV
- NumPy

You can install these libraries using pip:

```bash
pip install opencv-python numpy
```

# Usage

## 1) Load an Image

The code reads an image using OpenCV's cv2.imread() function. Make sure to specify the correct path to your image file.

```
image = cv2.imread('/content/cameraman.bmp')
cv2_imshow(image)
```

## 2) Input

Enter the Scaling Factor and Rotation Angle (in degrees) for Bilinear Interpolation and Nearest Neighbour Interpolation.

## 3) Save Results

The processed images are saved using cv2.imwrite().

```
cv2.imwrite('scaled_nn_image.jpg', scaled_nn_image)
cv2.imwrite('scaled_bilinear_image.jpg', scaled_bilinear_image)
cv2.imwrite('rotated_image_nn.jpg', rotated_image_nn)
cv2.imwrite('rotated_image_bilinear.jpg', rotated_image_bilinear)
```

## 4) Notes

- Ensure that the image path provided in cv2.imread() is correct.
- The code includes user input for scale factors and rotation angles.
- cv2_imshow() is used for displaying images in Google Colab.

## 5) References

- OpenCV Documentation
- NumPy Documentation
