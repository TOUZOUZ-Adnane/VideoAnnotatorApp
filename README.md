# VideoAnnotatorApp

An interactive Tkinter application for annotating video frames with labels and teams, saving the annotations in a structured JSON file format. The annotations are saved next to the video file in a JSON format.

## Features

- Load and play video files.
- Annotate specific frames with labels and teams.
- Save the annotations in a JSON file.
- Resume annotating by appending to an existing JSON file.

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/TOUZOUZ-Adnane/VideoAnnotatorApp.git
cd VideoAnnotatorApp
```
### 2. Create a virtual environment

It's recommended to create a virtual environment to keep dependencies isolated.

```bash
# Create a virtual environment
python -m venv venv

# Activate the environment
# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate
```

### 3. Install the required dependencies

Once the virtual environment is activated, install the required dependencies from `requirements.txt`:

```bash
# Ensure the virtual environment is activated, then run:
pip install -r requirements.txt
```

### 4. Start the application

To start the Video Annotator application, ensure your virtual environment is activated, then run the following command:

```bash
python tkinter_main.py
```

### 5. Using the Application

1. **Select a Video File**: When you start the application, a file dialog will open. Select the video file you want to annotate (supported formats: .mp4, .mkv).

2. **Play/Pause the Video**: Use the "Play/Pause" button to control video playback.

3. **Navigate Frames**: 
   - Click "Forward 10 Frames" to move forward in the video.
   - Click "Backward 10 Frames" to move backward.

4. **Annotate the Frame**:
   - Enter the label and team information in the provided input fields.
   - Click "Annotate Frame" to save the annotation for the current frame.

5. **Annotations Storage**: Annotations will be saved in a JSON file next to the selected video file. If the JSON file already exists, new annotations will be added to the existing file.

6. **Close the Application**: You can close the application by clicking the close button on the window.


### JSON Output Structure

The annotations for the video are saved in a JSON file with the following structure:

```json
{
    "UrlLocal": "video_filename",
    "UrlYoutube": "",
    "annotations": [
        {
            "gameTime": "00:05:30",
            "label": "PASS",
            "position": 680,
            "team": "away",
            "visibility": "visible"
        },
        {
            "gameTime": "00:10:15",
            "label": "DRIVE",
            "position": 2400,
            "team": "home",
            "visibility": "visible"
        }
    ]
}
```

## Contact

For any inquiries or further information, feel free to contact me via:
- [LinkedIn](https://www.linkedin.com/in/adnane-touzouz/)
- [Email](mailto:adnane.touzouz.ta@gmail.com)
