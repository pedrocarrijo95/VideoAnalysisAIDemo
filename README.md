# 🎥 VideoAnalysiAi

**VideoAnalysiAi** is a comprehensive notebook that analyzes human motion and facial expressions in a video. It draws human skeletons using pose estimation, detects abrupt movements, performs facial recognition, and generates a full report of the analysis.

---

## 🔍 Features

- ✅ **Pose Detection** with [MediaPipe](https://google.github.io/mediapipe/)
- ✅ **Abrupt Movement Detection** using landmark speed and pattern history
- ✅ **Facial Recognition** with [face_recognition](https://github.com/ageitgey/face_recognition)
- ✅ **Emotion Analysis** using [DeepFace](https://github.com/serengil/deepface)
- ✅ **Report Generation** summarizing:
  - Detected motions
  - Emotion frequency
  - Anomaly rate
  - Labeled activity types

---

## 🧠 Requirements

- Python 3.10+
- GPU runtime (mandatory for performance)

**Dependencies**:
```bash
pip install opencv-python mediapipe face_recognition deepface tf-keras tqdm
```

## 🗂 How to Run

### Clone the repository and open the VideoAnalysiAi.ipynb notebook.
### Update the SCRIPT_DIR variable with the full path to your working directory:

#### It must contain:

An images/ folder (for facial recognition reference images)
The input video
An output path for the processed result

```bash
# Example:
SCRIPT_DIR = "/content/drive/MyDrive/Project/"
```

Run the cells in order. Make sure to use Google Colab GPU or your local machine with a supported GPU.

## 📊 Example Output (Summary)

```bash
Summary of Detected Actions:
- Right arm raised: 13.74%
- Both arms raised: 6.05%
- Left arm raised: 6.78%
- Arms down: 73.42%

Summary of Detected Emotions:
- Happy: 31.38%
- Sad: 24.33%
- Neutral: 21.38%
- Fear: 10.82%
- Angry: 5.41%
- Surprise: 6.61%
- Disgust: 0.06%

Summary of Labeled Activities:
- Rest: 73.42%
- Raise both arms: 6.05%
- Raise left arm: 6.78%
- Raise right arm: 13.74%

Analysis Info:
- Total frames analyzed: 3326
- Anomalous movements detected: 171
- Frames with anomalies: 5.14%
```

## 💡 Use Cases

1. Surveillance analysis
2. Activity monitoring in sports or therapy
3. Emotion tracking during presentations or user studies
4. Crowd behavior anomaly detection

## 🚀 Ideas

1. Export CSV reports
2. Real-time webcam input
3. Dashboard with live stats

