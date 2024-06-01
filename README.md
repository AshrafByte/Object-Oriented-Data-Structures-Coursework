# Object-Oriented Data Structure Coursework

This repository contains my coursework for the Coursera course "Object-Oriented Data Structures in C++" by the University of Illinois. This project, MP1: Image Transform, involves creating a C++ class for handling pixel data in the HSL color space and using it to perform various image transformations.

## Project Overview

The project is divided into two main parts:

1. **HSLAPixel Class**: Implementation of a class to represent colored pixels in the HSL (Hue, Saturation, Luminance) color space.
2. **Image Transformations**: Using the `HSLAPixel` class and a provided `PNG` class to perform image transformations including grayscaling, illinifying, creating spotlights, and applying watermarks.

## Files in This Repository

### Provided by the Course

The following files and libraries were provided by the course creators to help structure and facilitate the project:

- `uiuc/PNG.h` and `uiuc/PNG.cpp`: A complete PNG class for handling image files.
- `tests/*`: Unit tests to validate the correctness of the implemented functions.
- `Makefile`: A makefile for compiling the project and the tests.
- `main.cpp`: The main driver program for running the image transformations.

### Implemented by Me

The following files were edited or created by me to complete the coursework:

- `uiuc/HSLAPixel.h` and `uiuc/HSLAPixel.cpp`: Implementation of the `HSLAPixel` class, representing pixels in the HSL color space.
- `ImageTransform.h` and `ImageTransform.cpp`: Implementation of the image transformation functions:
  - `grayscale`: Converts an image to grayscale.
  - `illinify`: Changes the hue of every pixel to Illini Orange or Illini Blue.
  - `spotlight`: Creates a spotlight effect centered at a given point.
  - `watermark`: Applies a watermark to an image based on a stencil image.

## Image Transformations

### Grayscale

Converts an image to grayscale by setting the saturation of every pixel to 0.

### Illinify

Changes the hue of every pixel to either Illini Orange (hue = 11) or Illini Blue (hue = 216), depending on which is closer.

### Spotlight

Creates a spotlight effect centered at `(centerX, centerY)`, reducing luminance based on distance from the center.

### Watermark

Applies a watermark to an image, increasing the luminance of the base image's pixels where the stencil image's pixels have maximum luminance.

## Compilation and Testing

To compile the project, navigate to the directory containing the `Makefile` and run : make

To run the unit tests, use: make test
./test

To clean up the compiled files, use: make clean


## Acknowledgements

I would like to acknowledge the University of Illinois and the course creators for providing the foundational code and structure for this project. The `PNG` class and the unit tests were provided as part of the course materials, enabling me to focus on implementing the specific transformations and the `HSLAPixel` class.





