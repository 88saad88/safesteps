# SafeSteps: Assistive Device for the Visually Impaired

SafeSteps is an innovative project designed to enhance accessibility for visually impaired individuals. By combining advanced vision algorithms, haptic feedback, and audio guidance, we aim to provide a hands-free device for safer and more efficient navigation.

---

## Table of Contents
- [Background](#background)
- [Features](#features)
- [System Architecture](#system-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [Contributors](#contributors)
- [Future Enhancements](#future-enhancements)

---

## Background

Traditional white canes, while effective, cannot detect ground hazards or obstacles beyond their physical reach. SafeSteps addresses this limitation by utilizing computer vision, tactile feedback, and audio instructions for better navigation.

---

## Features

- **Obstacle Detection**: Detects squares, crosses, and red lines to guide the user through corridors.
- **Haptic Feedback**: Vibrations alert the user when they are too close to red boundary lines.
- **Audio Guidance**: Provides real-time instructions (e.g., "Left", "Right", or "Straight").
- **Tilted Camera**: Captures the area directly in front of the user's feet.
- **Advanced Algorithms**:
  - Detects geometric shapes (squares and crosses).
  - Identifies corridors using red lines.
  - Calculates distances to objects for precise guidance.

---

## System Architecture

1. **Camera**: Captures real-time video of the environment.
2. **Raspberry Pi 4**: Processes video input using computer vision algorithms.
3. **Haptic Sensor**: Provides physical feedback for proximity warnings.
4. **Earphones**: Deliver audio guidance for navigation.
5. **Algorithms**:
   - Detect and classify shapes (squares and crosses).
   - Track corridor boundaries with red line detection.
   - Measure distances to ensure safe navigation.

---

## Installation

### Prerequisites
- **Hardware**:
  - Raspberry Pi 4 with PiJuice HAT (4-6 hours of battery life).
  - Camera module compatible with Raspberry Pi.
  - Haptic sensor connected to GPIO pins.
  - Earphones.
- **Software**:
  - Python 3.
  - Required Python libraries (see `requirements.txt`).

### Steps
1. Clone this repository:
   ```bash
   git clone https://gitlab.eurecom.fr/abbaoui/safesteps
   cd safesteps
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Connect the hardware components to the Raspberry Pi.

---

## Usage

1. Power on the Raspberry Pi and start the main script:
   ```bash
   python3 main.py
   ```
2. Show both hands to start or stop the algorithm.
3. Follow the corridor detected by the device:
   - Audio guidance will help you orient yourself.
   - Haptic feedback will warn you of proximity to red boundary lines.

---

## Future Enhancements

- **AI-Based Obstacle Classification**: Improve object and shape recognition accuracy.
- **Modular Design**: Simplify the addition of new features.
- **Mass Production**: Adapt the device for widespread commercial use.

---

## License

This project is open-source and available under the MIT License. For more information, see the `LICENSE` file.

---

SafeSteps: An innovative navigation solution for visually impaired individuals. ✨
