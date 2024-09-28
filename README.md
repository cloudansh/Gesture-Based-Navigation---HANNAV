# Hand Gesture Control System

## Overview

This project implements a hand gesture-based control system using OpenCV and MediaPipe. The system recognizes hand gestures and maps them to various actions such as controlling system brightness, volume, and performing mouse operations like click, scroll, and drag.

## Features

- **Mouse control**: Control mouse movement, clicks, right-clicks, and drags using hand gestures.
- **Pinch control**: Adjust system brightness or volume by pinching gestures.
- **Gesture recognition**: Detect and interpret various hand gestures such as:
  - **Fist**: Drag using mouse.
  - **V gesture**: Move the mouse cursor.
  - **Two-finger closed**: Double click.
  - **Pinch (Major/Minor)**: Control system brightness/volume or scroll.

## How It Works

- **Hand Gesture Detection**: The system uses MediaPipe to detect hand landmarks and recognizes gestures by analyzing finger positions.
- **Action Mapping**: Based on recognized gestures, actions like moving the mouse cursor, scrolling, adjusting volume, and brightness are triggered.

### Mouse Control

- **Moving the Mouse**: The index finger is used to move the mouse cursor across the screen. The system calculates the coordinates of the finger tip and maps them to the screen.
  
- **Click and Right-Click**: The system detects a two-finger closed gesture to perform a double-click. Other gestures allow for single and right-click actions.

### Brightness and Volume Control

- **Brightness Control**: When the thumb and index finger are pinched together (Major gesture), the system decreases or increases brightness based on the distance between the fingers.
  
- **Volume Control**: The same pinch gesture with different fingers (Minor gesture) is used to control the system volume, with the distance dictating the level.

### Scroll Control

- **Scroll Using Pinch**: Pinching and moving the hand up or down performs scrolling actions.

## Installation



1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository-url.git
   
## Remember to install all the Dependencies that are crucial for the program

2. Navigate into the project directory:

```bash
  cd your-repository-directory



