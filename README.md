# Text-to-Speech Converter using Python

A simple Python project that converts user-entered text into speech using the **Google Text-to-Speech (gTTS)** library. The generated speech is saved as an MP3 file and played directly in a Jupyter Notebook.

## Features

- Convert text to speech
- Save the output as an MP3 file
- Play audio inside Jupyter Notebook
- Simple and beginner-friendly project

## Technologies Used

- Python
- gTTS (Google Text-to-Speech)
- IPython Display

## Requirements

- Python 3.x
- gTTS
- IPython (for Jupyter Notebook)

Install the required package:

```bash
pip install gTTS
```

If needed, install IPython:

```bash
pip install ipython
```

## Code

```python
from gtts import gTTS
from IPython.display import Audio, display

text = input("Enter text: ")

tts = gTTS(text=text, lang="en")
tts.save("speech.mp3")

display(Audio("speech.mp3"))
```

## How to Run

1. Open the Python script or Jupyter Notebook.
2. Run the program.
3. Enter the text when prompted.
4. The program converts the text into speech.
5. The audio is saved as `speech.mp3` and played in the notebook.

## Example

**Input**

```
Enter text: Hello, welcome to my project!
```

**Output**

- A file named `speech.mp3` is created.
- The generated speech is played in the notebook.

## Project Structure

```
Text-to-Speech/
│── text_to_speech.py
│── speech.mp3
└── README.md
```

## Future Improvements

- Support multiple languages
- Allow users to choose the output filename
- Add speech speed control
- Build a GUI using Tkinter or Streamlit
- Convert text files into speech

## License

This project is open source and available under the MIT License.
