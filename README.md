<h1>Invisibility Cloak Effect with OpenCV</h1>

This project implements a real-time invisibility cloak effect using Python and OpenCV. By capturing the background and creating a mask based on a specific color (green in this case), the application allows the user to appear invisible against the captured backdrop.

## Features

- **Background Capture**: Captures a static background by averaging multiple frames, ensuring a smooth effect.
- **Color Masking**: Utilizes HSV color space to create a mask for the specified color range.
- **Real-time Processing**: Processes video frames in real time, allowing for interactive demonstration.
- **Morphological Transformations**: Applies morphological operations to clean up the mask for better results.

## Requirements

- Python 3.x
- OpenCV (`opencv-python`)
- NumPy

## Installation

To install the necessary packages, run:

```bash
pip install opencv-python numpy
```

## Usage

- Connect your camera.

- Run the script:

```bash
python invisibility_cloak.py
```
- Move out of the frame to capture the background.

- Wear a green shirt (or any object within the specified green color range) to see the invisibility effect.

- Press 'q' to exit the program.

## How It Works

- Capture Background: The program captures a series of frames to create a static background.
- Create Color Mask: It detects the specified color and creates a mask.
- Apply Cloak Effect: Combines the original frame and background using the mask, creating the invisibility effect.
