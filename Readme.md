# Virtual Mouse Gesture Controller

This project implements a virtual mouse that can be controlled using hand gestures. It leverages computer vision techniques and machine learning models provided by MediaPipe to detect and interpret hand movements, allowing you to control your computer's cursor and perform various actions using gestures.

## Features

- **Hand Gesture Recognition**: Detects various hand gestures such as fist, open palm, and specific finger movements.
- **Cursor Control**: Moves the cursor based on hand position.
- **Gesture-Based Actions**:
  - Fist: Click and drag.
  - Two fingers closed: Double click.
  - Pinch: Scroll and adjust system volume/brightness.
  - Specific finger gestures for right-click and other actions.
- **Graphical User Interface (GUI)**: A user-friendly interface to start and stop the gesture recognition.

## Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/virtual-mouse-gesture-controller.git
    cd virtual-mouse-gesture-controller
    ```

2. **Install the required packages**:
    ```sh
    pip install -r requirements.txt
    ```

    Ensure the following libraries are installed:
    - OpenCV
    - MediaPipe
    - PyAutoGUI
    - Math
    - Enum
    - Pycaw
    - Google Protobuf
    - Screen Brightness Control
    - Pynput
    - Tkinter
    - PIL (Pillow)

## Usage

1. **Run the application**:
    ```sh
    python main.py
    ```

2. **Using the GUI**:
    - A window will appear with a button labeled "Track Mouse". Click this button to start the gesture recognition.
    - You can also press the `Enter` key to start the gesture recognition.

3. **Performing gestures**:
    - Move your hand in front of the camera to control the cursor.
    - Use specific gestures to perform actions like clicking, dragging, scrolling, and adjusting volume/brightness.

## Gesture Controls

- **Fist**: Click and drag.
- **Two Fingers Closed**: Double click.
- **Pinch**:
  - Horizontal pinch: Scroll horizontally.
  - Vertical pinch: Scroll vertically.
- **V Gesture**: Move cursor.
- **Index Finger**: Right-click.
- **Middle Finger**: Single click.

## Configuration

- **Colors**: You can customize the colors for fingertip and hand landmarks by modifying the `TIPCOLOR` and `HANDCOLOR` variables.
- **Camera Settings**: Adjust camera resolution and frame settings in the `GestureController` class.

## Code Overview

- **GestureController Class**: Manages the initialization and processing of hand gestures using MediaPipe.
- **HandRecog Class**: Recognizes and encodes hand gestures based on landmark positions.
- **Controller Class**: Maps gestures to system controls (mouse movements, clicks, scrolls, volume, and brightness adjustments).
- **GUI**: Built using Tkinter, providing a simple interface to start and stop gesture recognition.

## Troubleshooting

- Ensure your webcam is properly connected.
- Make sure you have all required libraries installed.
- Adjust the lighting in your environment for better hand detection accuracy.

## Contributing

Feel free to fork this repository, create new features, fix bugs, or improve the documentation. Pull requests are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

