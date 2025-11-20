# IMAGE-TRANSFORMATIONS
## Aim

To implement and demonstrate various Geometric Transformations (Scaling, Rotation, Translation, Affine) on images using Python and OpenCV.

## Software Required

1. Anaconda - Python 3.x
2. OpenCV
3. Matplotlib
4. NumPy

## Features

- **Scaling (Resizing):** Implements image resizing using various interpolation methods (e.g., cv2.INTER_LINEAR, cv2.INTER_CUBIC).

- **Translation:** Shifts the image along the x and y axes using a 2 x 3 transformation matrix.

- **Rotation:** Rotates the image about a specified center point by a given angle.

- **Affine Transformation:** Preserves parallelism and ratios of distances, useful for shear and general linear mapping.

## Algorithm:

### Step 1: Load Image and Define Parameters

Load the input image. Define necessary parameters like rotation angle, translation vectors (Tx, Ty), and scaling factors (sx, sy).

### Step 2: Implement Translation

Create the 2 x 3 translation matrix M. Apply cv2.warpAffine using M to shift the image.

### Step 3: Implement Rotation

Use cv2.getRotationMatrix2D to generate the rotation matrix. Apply cv2.warpAffine to rotate the image around a central pivot.

### Step 4: Implement Scaling

Use cv2.resize to perform scaling up or down, specifying the interpolation method for smoother results.

## Step 5: Display Results

Display the original image and all transformed results (scaled, rotated, translated, affine) for comparative analysis.
