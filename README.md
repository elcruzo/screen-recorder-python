# Python Screen Recorder

This repository contains a simple script that allows you to record your computer screen and save it as a video file.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Contributions](#contributions)
- [License](#license)

## Introduction

This Python Screen Recorder is a simple script that allows you to record your computer screen and save it as a video file. This project uses Python along with the OpenCV and PyAutoGUI libraries to capture the screen and create a video recording.

## Features

- Real-time video streaming from a camera to a remote device.
- Two-way communication between a camera device and a remote viewer.
- Easy setup for local network communication.

## Requirements

To use this script, you need the following:

- Python 3.6 or higher installed on both the camera and remote devices.
- The `time` module (usually included in Python standard library)
- The `numpy` library, which can be installed using pip:
  ```bash
  pip install numpy
  ```
- The OpenCV (`cv2`) library, which can be installed using pip:
  ```bash
  pip install opencv-python
  ```
- The PyAutoGUI library, which can be installed using pip:
  ```bash
  pip install pyautogui
  ```

## Installation

1. Ensure you have Python 3.x installed. You can check by running:

   ```bash
   python3 --version
   ```
   If Python is not installed, you can download it from the official [Python website](https://www.python.org/downloads/).

2. Clone this repository to to both the camera and remote devices or download it as a ZIP file:

   ```bash
   git clone https://github.com/elcruzo/screen-recorder-python.git
   ```
3. Navigate to the project directory:

   ```bash
   cd screen-recorder-python
   ```
4. Modify the script as needed. You can customize the screen size, frame rate, and output filename by editing the following lines in index.py:

   ```bash
   SCREEN_SIZE = (1920, 1080)
   fourcc = cv2.VideoWriter_fourcc(*"XVID")
   out = cv2.VideoWriter("output.avi", fourcc, 20.0, SCREEN_SIZE)
   ```
5. Save your changes

## Usage

1. Run the script using the following command::
   ```bash
   python index.py
   ```
2. The script will start recording your screen.
3. To stop the recording, press `Ctrl+C` in the terminal where the script is running.
4. The recorded video will be saved as [output.avi](output.avi) in the project directory.

## Contributions

Contributions to this repository are welcome! If you have any improvements or feature suggestions, feel free to fork this repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Have fun exploring my Screen Recorder Application! If you have any questions or run into issues, don't hesitate to ask for help.

   
