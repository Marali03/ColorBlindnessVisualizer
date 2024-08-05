# ColorBlindnessVisualizer
## Overview

This project demonstrates a simple application to simulate various types of color blindness. It takes an input image and applies transformations to simulate how the image would appear to individuals with different types of color vision deficiencies.

## Features

- **Color Blindness Simulation**: Simulates various types of color blindness including:
  - Protanopia
  - Protanomaly
  - Deuteranopia
  - Deuteranomaly
  - Tritanopia
  - Tritanomaly
  - Achromatopsia
  - Achromatomaly
- **Image Processing**: Applies color transformations to simulate the visual experience of color blindness.
- **User Input**: Allows users to specify the image file path and type of color blindness to simulate.
- **Output**: Displays both the original and simulated images, and saves the simulated image to disk.

## Requirements

- `opencv-python`: For image processing and displaying.
- `numpy`: For numerical operations and matrix manipulations.

## Usage

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/Marali03/ColorBlindnessVisualizer.git
    cd ColorBlindnessVisualizer
    ```

2. **Install Required Packages**:

    You can install the required packages using `pip`:

    ```bash
    pip install opencv-python numpy
    ```

3. **Run the Program**:

    Execute the script using Python:

    ```bash
    python ColorBlindnessVisualizer.py
    ```

    The script will prompt you to enter:
    - The path to the image file (e.g., `C:\Users\XXXY\Downloads\image.jpg`).
    - The type of color blindness (e.g., `'protanopia'`, `'deuteranopia'`, etc.).

    The script will display the original and simulated images, and save the simulated image as `simulated_<deficiency_type>.jpg`.

## How It Works

1. **Get the Transformation Matrix**: Based on the user's input, the script retrieves a matrix that represents how colors are perceived by individuals with different types of color blindness.
2. **Apply the Transformation**: The script applies this matrix to the input image to simulate the color blindness effect.
3. **Display and Save**: It then displays the original and simulated images, and saves the simulated image to disk.

## Example

For an example usage, enter the following when prompted:
- **Image Path**: `C:\Users\XXXY\Downloads\image.jpg`
- **Color Blindness Type**: `protanopia`

The program will show the original image and the simulated image as perceived by someone with protanopia, and save the result as `simulated_protanopia.jpg`.

