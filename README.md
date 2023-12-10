# Wiener Filter - Image Denoising and Deblurring

This project focuses on implementing a Wiener filter for image denoising and deblurring, providing a comprehensive solution to enhance image quality. The following sections detail the key steps and implementation specifics.

## Approach

### 1. Image Denoising

#### 1.1 Wiener Filter Creation

- **Wiener Filter:** Developed a Wiener filter to address image denoising challenges.
  
- **Wiener Filter Equation:** Implemented the Wiener filter equation, taking into account the power spectral density of the noise and the signal in both the frequency and spatial domains.

- **Noise Estimation:** Estimated the noise variance to adapt the Wiener filter to the specific noise characteristics in the image.

#### 1.2 Denoising Process

- **Frequency Domain Transformation:** Transformed the image and filter to the frequency domain using the Fast Fourier Transform (FFT).

- **Wiener Filter Application:** Applied the Wiener filter to the image in the frequency domain.

- **Inverse FFT:** Inverse transformed the filtered image back to the spatial domain.

### 2. Image Deblurring

#### 2.1 Blur Kernel Estimation

- **Blur Kernel Identification:** Implemented methods for estimating the blur kernel, crucial for effective deblurring.

#### 2.2 Deblurring Process

- **Wiener Deconvolution:** Applied Wiener deconvolution to restore the image, considering the estimated blur kernel.

### 3. Optimization and Performance

- **Matrix Multiplication:** Optimized the implementation for efficiency by converting O(n^2) loops to matrix multiplication where applicable.

## Usage

Provided instructions or code snippets for users to apply the Wiener filter for their image denoising and deblurring needs.

## Implementation Specifics

- **Selection of Parameter "k":** Choosing the parameter "k" for the adaptive nature of the Wiener filter presented a significant challenge. The value of "k" impacts the trade-off between preserving image details and reducing noise. Experimentation and analysis were performed to find an optimal "k" for different types of images and noise characteristics.

## Acknowledgments

[1] Defocus Blur, Neel Joshi <br>
Microsoft Corporation, Redmond, WA, USA
