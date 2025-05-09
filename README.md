# 🎙️ Speech Recognition Projects Suite

A collection of deep learning-based audio recognition systems focused on voice-driven automation and safety.  
This suite includes:

- 😨 **Fear Detection** from voice for triggering security alerts
- 🗣️ **Speech-to-Text** transcription using the Google Speech Command dataset
- 🔢 **Digit Recognition (0–9)** from spoken audio using the same dataset

---

## 🔐 Project 1: Fear Detection for Security Alert

### 📌 Description:
Detects **fear emotion** in human voice using audio classification. Upon detection, it can **trigger a security alert** such as logging, sound alarms, or sending emails.

### 💡 Use Case:
- Smart home intrusion alerts  
- Panic detection in surveillance  
- Emergency call systems  

### 🛠 Features:
- Preprocessing with **MFCC**
- Model: CNN or MLP classifier
- Real-time or batch audio analysis

### ▶️ Run:
```bash
python fear_alert/alert_trigger.py --audio path/to/fear_audio.wav
🗣️ Project 2: Speech-to-Text using Google Speech Command
📌 Description:
Performs simple speech-to-text transcription using voice command clips from the Google Speech Command dataset.

💡 Use Case:
Voice-controlled UI

Command recognition for devices or software

🛠 Features:
Audio preprocessing (MFCC / Spectrogram)

Trained CNN or CRNN model for classification

Outputs recognized keywords as text

▶️ Run:
bash
Copy
Edit
python speechtotext/transcribe.py --audio path/to/command.wav
🔢 Project 3: Digit Recognition (0–9)
📌 Description:
Recognizes digits (zero through nine) spoken in audio using the Google Speech Command dataset.

💡 Use Case:
Spoken digit entry for authentication

Smart calculators

Voice-based phone dialing

🛠 Features:
Trained CNN on MFCC features

Supports inference on custom audio samples

Accuracy > 90% with clean audio

▶️ Run:
bash
Copy
Edit
python digitrecog/train_model.py
python digitrecog/predict_digit.py --audio path/to/digit.wav
🧱 Project Structure
Copy
Edit
speech-recognition-suite/
├── fear_alert/
│   ├── dataset/
│   ├── feature_extract.py
│   ├── model.py
│   └── alert_trigger.py

├── speechtotext/
│   ├── dataset/
│   ├── train.py
│   ├── model.py
│   └── transcribe.py

├── digitrecog/
│   ├── dataset/
│   ├── preprocessing.py
│   ├── train_model.py
│   └── predict_digit.py

├── utils/
│   ├── audio_utils.py
│   └── visualization.py

└── README.md
📦 Installation
Install all dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Key Libraries:

TensorFlow or PyTorch

librosa, numpy, matplotlib

scikit-learn

pyaudio, soundfile

📊 Visualizations
Waveforms and Spectrograms

Model performance graphs (loss/accuracy)

Confusion matrices for classification

Run visualizations:

bash
Copy
Edit
python utils/visualization.py
🔮 Future Enhancements
Real-time microphone input

Emotion classification beyond fear (anger, sadness, etc.)

Mobile app and edge deployment (Raspberry Pi)

Multilingual speech support

