Python GUI Google Search Application
This is a simple desktop application built with Python that provides a graphical user interface (GUI) to perform Google searches. Users can either type their search query or use their voice to search directly from the desktop.
Project Overview
The application presents a small window with two main options: "Type Search" and "Voice Search". It is designed for quick and easy access to Google without needing to open a web browser first. The script leverages several Python libraries to create the GUI, handle user input, process voice commands, and open the search results in the user's default web browser.
Features
Simple Graphical User Interface (GUI): A clean and straightforward window built with tkinter.
Text-Based Search: A dialog box prompts the user to type in their search query.
Voice-Based Search: Uses the computer's microphone to listen for a voice command, converts the speech to text, and performs the search.
Cross-Platform: As it is built with Python and tkinter, it should run on Windows, macOS, and most Linux distributions.
Automatic Browser Integration: Opens the search results directly in the user's default web browser.
Technologies and Libraries Used
Python: The core programming language for the application.
Tkinter: Python's standard GUI library, used to create the main window, buttons, and dialog box.
PyWhatKit: A simple and powerful library used here to instantly perform a Google search from a text string.
SpeechRecognition: A library for performing speech recognition, with support for several engines and APIs. This project uses the Google Speech Recognition API.
PyAudio: Required by SpeechRecognition to access the microphone hardware (works as a dependency).
Webbrowser: A Python library used to open the search URL in the default web browser.
Prerequisites
Before running the application, you need to have Python installed on your system. You will also need to install the required third-party libraries. A microphone is necessary to use the "Voice Search" feature.
Installation
Clone the repository or download the script:
Save the Python script (e.g., app.py) to a local directory.
Install the required Python packages:
Open your terminal or command prompt and install the necessary libraries using pip.
Generated sh
pip install requests
pip install pywhatkit
pip install SpeechRecognition
pip install PyAudio
Use code with caution.
Sh
Note: Installing PyAudio can sometimes be tricky. If you encounter issues, you may need to install it using a package manager like Homebrew on macOS (brew install portaudio) or by downloading a pre-compiled Wheel file (.whl) for your specific Python version and system architecture on Windows.
How to Run the Application
Navigate to the script's directory:
Open a terminal or command prompt and use the cd command to go to the folder where you saved the script.
Generated sh
cd path/to/your/script
Use code with caution.
Sh
Execute the Python script:
Generated sh
python your_script_name.py
Use code with caution.
Sh
The application window will appear on your screen.
How to Use the Application
Once the application is running, you will see a window with two buttons.
For Text Search:
Click the typesearch button.
A dialog box will appear asking you to "enter word to search:".
Type your query into the text field and click OK.
Your default web browser will open with the Google search results for your query.
For Voice Search:
Ensure your microphone is connected and enabled.
Click the voicesearch button.
The application will start listening. Say your search query clearly into the microphone.
Once you stop speaking, the application will process the audio.
Your default web browser will open with the Google search results for what you said. If your speech cannot be recognized, an error message will be printed to the console.
