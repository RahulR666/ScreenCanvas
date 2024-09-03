# ScreenCanvas

ScreenCanvas is a Python-based virtual drawing application that uses hand gestures to draw on a canvas. The application utilizes OpenCV and MediaPipe to track hand movements in real-time, allowing users to select colors, draw, and clear the canvas using simple hand gestures.

## Features

- **Real-time Hand Gesture Recognition**: Tracks hand landmarks to detect gestures and control drawing.
- **Virtual Canvas Drawing**: Allows users to draw on a digital canvas using finger movements.
- **Dynamic Color Selection**: Switch between multiple colors (blue, green, red, yellow) using hand gestures.
- **Canvas Clearing**: Clear the canvas with a simple gesture.

## Tools, Frameworks, and Libraries

### Programming Language
- **Python**: The main language used for the development of the application.

### Libraries
- **OpenCV (cv2)**: Used for real-time video processing, drawing operations, and creating the canvas interface.
- **MediaPipe**: Provides accurate hand and finger landmark detection.
- **NumPy**: Handles numerical operations, specifically for image processing tasks.
- **Collections (deque)**: Manages drawing points efficiently using double-ended queues.

### Frameworks
- **MediaPipe**: Acts as a framework for hand tracking and gesture recognition.

### Tools
- **Webcam**: Captures real-time video input for processing.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/screencanvas.git
    cd screencanvas
    ```

2. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the application**:
    ```bash
    python screencanvas.py
    ```

## How It Works

- The application captures real-time video from your webcam and processes the frames to detect hand gestures.
- By tracking the index finger's position, the application allows you to draw on a canvas.
- Gesture-based commands enable you to select colors, draw, and clear the canvas.

## Usage

1. **Run the application**: 
   Ensure your webcam is connected and run the `screencanvas.py` script.
   
2. **Start Drawing**:
   - Move your index finger to draw on the canvas.
   - To change colors, move your hand over the color boxes at the top of the screen.
   - To clear the canvas, move your hand over the "CLEAR" box.

3. **Exit the application**:
   Press the `q` key to quit the application.

## Future Enhancements

- Add support for saving the canvas as an image file.
- Improve gesture recognition accuracy and add more gestures for different functionalities.
- Implement a more sophisticated user interface for easier interaction.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to discuss improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, please contact [your.email@example.com](mailto:your.email@example.com).

