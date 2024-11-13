# Image-Noise-Removal-by-Matlab

This code reads an image file from a specified path using the imread() function and stores it in the variable `I`.The image is then separated into its red, green, and blue channels using the indexing notation `I(:, :, 1)`, `I(:, :, 2)`, and `I(:,:,3)`, respectively, and stored in the variables red_channel, green_channel, and blue_channel.

The code applies a 3x3 median filter to each of the color channels using the medfilt2() function. Median filtering is a technique for removing noise from an image by replacing each pixel value with the median of the neighboring pixels. The resulting filtered channels are stored in the same variables as before.

The filtered channels are then concatenated back together using the cat() function and the variable F. The resulting image, with reduced noise, is displayed side by side with the original image using the subplot() function and the imshow() function with the title() function to display the titles of each subplot. The first subplot displays the original noisy image, while the second subplot displays the image after noise removal.

## Getting Started

To get started with this code, make sure you have MATLAB or Octave installed on your system. Clone or download this repository to your local machine, and run the `main.m` file to execute the code.

The image file to be processed should be stored in the same directory as the code file, or the file path should be specified in the `imread()` function.

## Requirements
- MATLAB R2016a or later
- Octave 5.2.0 or later

## Usage
1) Place the image file to be processed in the same directory as the code file, or specify the file path in the imread() function.
2) Open MATLAB or Octave.
3) Navigate to the directory containing the `main.m` file.
4) Run the script using the command `main` in the command window.
5) The original and filtered images will be displayed side by side.

## Results:

<img width="368" alt="image" src="https://user-images.githubusercontent.com/68495520/236303748-00c9aaad-2440-42dd-a338-c2ffe22afc51.png">
