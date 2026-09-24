# ScreenCanvas

A real-time gesture-controlled virtual drawing application built with Python, OpenCV, and MediaPipe.

ScreenCanvas uses hand-landmark tracking to let users draw on a digital canvas using finger movements, switch colors through gesture-based interaction, clear the canvas, and interact with the application without a mouse or touchscreen.

---

## Overview

The project combines computer vision and human-computer interaction to create a touchless drawing interface.

A webcam captures the user's hand in real time. MediaPipe detects and tracks hand landmarks, while OpenCV processes the video stream and renders the drawing canvas.

The position of the index finger is used as the primary drawing input.

---

## Features

- Real-time hand landmark detection
- Gesture-controlled drawing
- Virtual drawing canvas
- Dynamic color selection
- Multiple drawing colors
- Gesture-based canvas clearing
- Real-time webcam processing
- Touchless human-computer interaction

---

## How It Works

The application follows the pipeline:

```text
Webcam Input
     |
     v
Frame Capture
     |
     v
Hand Landmark Detection
     |
     v
Finger Position Tracking
     |
     v
Gesture Interpretation
     |
     +--------------------+
     |                    |
     v                    v
Drawing Input        UI Interaction
     |                    |
     v                    v
Canvas Update       Color / Clear
     |
     v
Rendered Output
```

---

## Hand Tracking

MediaPipe is used to detect and track hand landmarks from each webcam frame.

The application tracks the index finger position and uses its movement to determine where drawing should occur on the virtual canvas.

---

## Gesture-Based Interaction

Different regions and hand movements are used to control the application.

### Drawing

Move the index finger across the drawing region to create strokes on the canvas.

### Color Selection

Move the hand over the color-selection areas at the top of the interface to change the active drawing color.

Available colors include:

- Blue
- Green
- Red
- Yellow

### Clear Canvas

Move the hand over the `CLEAR` region to erase the current drawing.

---

## Technologies

- Python
- OpenCV
- MediaPipe
- NumPy
- Collections `deque`
- Computer Vision
- Hand Tracking
- Gesture Recognition

---

## Repository Structure

```text
ScreenCanvas/
├── ScreenCanvas.py
├── README.md
└── LICENSE
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/RahulR666/ScreenCanvas.git
cd ScreenCanvas
```

Install the required dependencies:

```bash
pip install numpy opencv-python mediapipe
```

---

## Running the Application

Ensure that a webcam is connected, then run:

```bash
python ScreenCanvas.py
```

Press:

```text
q
```

to exit the application.

---

## Usage

1. Launch the application.
2. Position your hand clearly in front of the webcam.
3. Move your index finger to draw on the canvas.
4. Move your hand over one of the color-selection regions to change the drawing color.
5. Move your hand over the `CLEAR` region to reset the canvas.
6. Press `q` to quit.

---

## Demo

<!-- ADD DEMO GIF OR SCREENSHOT HERE -->

A short GIF demonstrating drawing, color selection, and canvas clearing will be added here.

Example:

```markdown
![ScreenCanvas Demo](results/screencanvas_demo.gif)
```

---

## Future Improvements

Potential improvements include:

- saving completed drawings as image files
- adding additional gesture commands
- improving gesture robustness
- supporting brush-size control
- adding an eraser mode
- improving the user interface
- supporting multiple hands
- adding gesture-based undo and redo
- improving performance under different lighting conditions

---

## License

This project is licensed under the MIT License.

See the `LICENSE` file for details.

---

## Author

**Rahul Rathnam**

Robotics Software Engineer  
Localization | Perception | Sensor Fusion | Autonomous Systems

GitHub: [RahulR666](https://github.com/RahulR666)
