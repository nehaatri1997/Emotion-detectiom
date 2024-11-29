# Emotion-detectiom

This project uses Hugging Face Transformers to analyze emotions from text input. It leverages the pre-trained model j-hartmann/emotion-english-distilroberta-base for accurate emotion classification. Additionally, it includes optional camera integration for capturing text input to analyze emotions.

# Features
Text-Based Emotion Detection:
Detect emotions such as joy, sadness, anger, surprise, etc., from user-provided text.
Camera Integration:
Captures a single frame from the camera (optional) to analyze text for emotions.
Real-Time Emotion Analysis:
Provides probability scores for each detected emotion.

# Installation
1. Clone the Repository
git clone https://github.com/your-repo-name/emotion-detection.git
cd emotion-detection
2. Install Required Libraries
Install the dependencies listed in the script:
pip install transformers torch opencv-python

# Usage
1. Run the Script
python emotion_detection.py
2. Text-Based Emotion Detection
Enter text samples directly in the script's texts array.

Example:
texts = [
    "I am so happy today!",
    "I feel really sad about what happened.",
    "I'm furious at the situation!",
    "I'm surprised and excited about the news!"
]
The output will display detected emotions for each input text:
Text: I am so happy today!
Joy: 0.85
Sadness: 0.05
Anger: 0.03
Surprise: 0.07
3. Camera Integration
Enable the camera by running the capture_and_analyze() function.
The script captures a frame and analyzes text from the pre-defined texts array.

File Structure
emotion_detection/
│
├── emotion_detection.py      # Main Python script for emotion detection
└── README.md                 # Documentation file

# Customization
Add Custom Text: Modify the texts array to include your desired text samples for analysis.
Camera Integration: Ensure your camera is properly connected for the capture_and_analyze() function to work.
