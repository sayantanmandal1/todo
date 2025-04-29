<<<<<<< HEAD
# Sign Language Recognition Web Interface

This project provides a web interface for sign language recognition, allowing users to convert sign language to text and speech using either uploaded images or live camera streaming.

## Features

- Live camera streaming for real-time sign language recognition
- Image upload functionality for processing stored images
- Text display of recognized letters, words, and sentences
- Speech output for recognized text
- Spell-checking to improve accuracy
- User-friendly interface with intuitive controls

## Project Structure

```
sign-language-web/
├── app.py                  # Main Flask application
├── static/
│   ├── uploads/            # Storage for uploaded images
│   └── temp/               # Temporary storage for generated audio files
├── templates/
│   └── index.html          # Base HTML template
├── trained_model_graph.pb  # Pre-trained TensorFlow model
└── training_set_labels.txt # Labels for the model
```

## Requirements

- Python 3.6+
- Flask
- TensorFlow
- OpenCV
- gTTS (Google Text-to-Speech)
- NumPy
- Flask-CORS

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd sign-language-web
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Ensure you have the trained model and labels files:
   - Place your `trained_model_graph.pb` in the project root
   - Place your `training_set_labels.txt` in the project root

   Note: Update the paths in `app.py` if your files are located elsewhere.

4. Create required directories:
   ```
   mkdir -p static/uploads static/temp
   ```

## Running the Application

1. Start the Flask application:
   ```
   python app.py
   ```

2. Open your web browser and navigate to:
   ```
   http://localhost:5000
   ```

## Usage Instructions

### Live Camera Mode
1. Click "Start Camera" to enable your webcam
2. Position your hand showing a sign within the green box
3. Click "Capture Sign" to manually recognize a sign, or
4. Enable "Real-Time Recognition" for continuous detection
5. Use "Add Space" to complete words and "Delete Last Letter" to correct mistakes

### Upload Image Mode
1. Click "Choose Image" to select an image file
2. Click "Process Image" to recognize the sign in the image

### Output Controls
- "Add Space": Completes the current word and adds a space
- "Delete Last Letter": Removes the last recognized letter
- "Clear All": Resets all recognized text
- "Speak Text": Reads the recognized text aloud

### Settings
- "Enable Spell Check": Automatically corrects common spelling mistakes
- "Auto-Speak Words": Automatically reads words aloud when completed

## Integration with Existing Code

This web interface integrates with your existing sign language recognition code using a Flask backend. The core functionality from your original code has been preserved and enhanced with web capabilities.

## Customization

- To add more words to the spell-checking dictionary, modify the `word_dictionary` in `app.py`
- To adjust the recognition sensitivity, modify the threshold values in the `predict_sign` function

## License

[Your License Here]

## Acknowledgments

- Based on the Unvoiced project for sign language recognition
- Uses TensorFlow for neural network processing
- Google Text-to-Speech for audio output
=======
# Task Master - Modern To-Do Application

![image](https://github.com/user-attachments/assets/64c3dd14-4d9a-4b06-a77f-aa27f05eeac3)


A sleek, modern, and aesthetically pleasing to-do list application with an animated 3D background and glass morphism design elements.

## Features

- **Stunning 3D Background**: Animated floating cubes with parallax effect that reacts to mouse movement
- **Modern UI Design**: Implements glass morphism, subtle animations, and gradient accents
- **Task Management**: Add, complete, and delete tasks with smooth animations
- **Filtering System**: Easily switch between all, active, and completed tasks
- **Persistent Storage**: Tasks are saved to local storage so they persist between sessions
- **Responsive Design**: Looks great on devices of all sizes
- **Interactive Elements**: Beautiful custom checkboxes and hover effects

## Technologies Used

- HTML5
- CSS3 (with animations and transitions)
- JavaScript (ES6+)
- Local Storage API

## Setup and Installation

This is a front-end only application that runs directly in the browser without any build steps or dependencies.

### Option 1: Quick Start

1. Simply download the HTML file
2. Open it with any modern web browser

### Option 2: Host It Yourself

1. Download the HTML file
2. Place it on your web server or hosting platform
3. Access it via your domain

## How to Use

1. **Add a Task**: Type your task in the input field and press Enter or click the "Add" button
2. **Mark as Complete**: Click the checkbox next to a task to mark it as complete
3. **Delete a Task**: Click the "×" button next to a task to remove it
4. **Filter Tasks**:
   - Click "All" to show all tasks
   - Click "Active" to show only uncompleted tasks
   - Click "Completed" to show only completed tasks
5. **Clear Completed**: Remove all completed tasks at once with the "Clear completed" button

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Customization

The application can be easily customized:

- **Colors**: Modify the gradient colors in the CSS
- **Animation Speed**: Adjust animation duration values in the CSS
- **Background Elements**: Change the number of floating cubes in the JavaScript

## Future Enhancements

- Drag and drop reordering of tasks
- Categories and tags for tasks
- Due dates and reminders
- Dark/light theme toggle
- Cloud synchronization

## Contributing

Feel free to fork this project and submit pull requests. You can also open issues for bugs or feature requests.

## License

MIT License

## Credits

- Fonts: [Poppins](https://fonts.google.com/specimen/Poppins) from Google Fonts
- Design Inspiration: Modern glass morphism and neumorphism UI trends

---

Made with ❤️ by [Sayantan]

>>>>>>> 770f56d746cf90558eb31156172d31439a730215
